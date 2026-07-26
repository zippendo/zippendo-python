# Zippendo Python SDK

Official Python client for the [Zippendo](https://zippendo.com) shipping & logistics API. Models are
pydantic v2, so requests and responses are both type-hinted and validated at runtime. Requires
Python 3.8+.

## Install

```sh
pip install zippendo
```

## Authentication

Create an API token in your Zippendo dashboard (**Settings → API tokens**) — a Bearer token prefixed
with `zipp_`. Pass it as `access_token`:

```python
import os
import zippendo

config = zippendo.Configuration(access_token=os.environ["ZIPPENDO_API_TOKEN"])
```

The base URL defaults to `https://api.zippendo.com`.

## Resources & clients

The API is split into resource clients — `ShipmentsApi`, `OrdersApi`, `CarriersApi`, `AddressesApi`,
`RulesApi`, `WebhooksApi`, `TokensApi`, and more. Create an `ApiClient` from your config, then the
resource clients you need:

```python
with zippendo.ApiClient(config) as client:
    shipments = zippendo.ShipmentsApi(client)
    orders = zippendo.OrdersApi(client)
```

## The `org_id` parameter

Every call takes an `org_id` (your organization ID, found in the dashboard). It is explicit on each
call by design: one API token can be granted access to multiple organizations, and `org_id` selects
which one the request acts on.

## Listing & pagination

List endpoints accept `page` (1-based) and `limit`, and return a page with `data` plus `total`,
`page`, `limit`, and `total_pages`:

```python
with zippendo.ApiClient(config) as client:
    shipments = zippendo.ShipmentsApi(client)
    result = shipments.list_shipments("org_8f3kd92ld0", page=1, limit=50)
    print(result.data)                       # list[Shipment]
    print(result.total, result.total_pages)  # pagination metadata
```

## Creating resources

```python
with zippendo.ApiClient(config) as client:
    orders = zippendo.OrdersApi(client)
    order = orders.create_order(
        "org_8f3kd92ld0",
        zippendo.CreateOrderRequest(
            order_number="1001",
            order_channel_id="chan_7d2k1",
            order_lines=[zippendo.CreateOrderRequestOrderLinesInner(name="T-shirt", quantity=2)],
        ),
    )
    print(order.id)
```

See [`./docs`](./docs) for the full request/response shape of every operation.

## Error handling

Non-2xx responses raise `ApiException`. The body is Zippendo's canonical `{ code, error, message }` —
branch on the machine-readable `code`:

```python
from zippendo.rest import ApiException

try:
    shipments.get_shipment("org_8f3kd92ld0", "shp_missing")
except ApiException as e:
    print(e.status, e.body)   # e.body contains the JSON, e.g. {"code": "SHIPMENT_NOT_FOUND", ...}
```

## Configuration

Point the client at a different environment by overriding `host`:

```python
config = zippendo.Configuration(
    access_token=os.environ["ZIPPENDO_API_TOKEN"],
    host="https://staging.api.zippendo.com",
)
```

## Reference

Full per-endpoint and per-model documentation is in [`./docs`](./docs). Hosted reference:
<https://www.zippendo.com/docs/api-reference/overview>.

## License

[MIT](./LICENSE.md)
