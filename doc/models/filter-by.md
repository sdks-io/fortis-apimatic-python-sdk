
# Filter By

*This model accepts additional fields of type Any.*

## Structure

`FilterBy`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `key` | `str` | Required | Resource key to filter by |
| `operator` | [Operator1](../../doc/models/operator-1.md) | Required | This is a container for one-of cases. |
| `value` | float \| str \| bool | Required | This is a container for one-of cases. |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "key": "first_name",
  "operator": "<=",
  "value": "Fred",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

