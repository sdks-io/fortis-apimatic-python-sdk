
# Settings

*This model accepts additional fields of type Any.*

## Structure

`Settings`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `enabled` | `bool` | Optional | Enabled |
| `columns` | `float` | Optional | Columns |
| `rows` | `float` | Optional | Rows |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "enabled": true,
  "columns": 1.0,
  "rows": 1.0,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

