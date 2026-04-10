
# Field

*This model accepts additional fields of type Any.*

## Structure

`Field`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `field` | `str` | Optional | Field name used on the sort |
| `order` | [`Order`](../../doc/models/order.md) | Optional | - |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "field": "last_name",
  "order": "asc",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

