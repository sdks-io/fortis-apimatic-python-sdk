
# Pagination

Pagination info

*This model accepts additional fields of type Any.*

## Structure

`Pagination`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `mtype` | [`Type3`](../../doc/models/type-3.md) | Optional | - |
| `total_count` | `int` | Optional | Total records count |
| `page_count` | `int` | Optional | Total page count |
| `page_number` | `int` | Optional | Current page |
| `page_size` | `int` | Optional | Page size |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "total_count": 423,
  "page_count": 42,
  "page_number": 6,
  "page_size": 10,
  "type": "Pagination",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

