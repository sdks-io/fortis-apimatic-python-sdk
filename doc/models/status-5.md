
# Status 5

*This model accepts additional fields of type Any.*

## Structure

`Status5`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `response_code` | `str` | Optional | Response code for API response.<br><br>**Constraints**: *Maximum Length*: `20` |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "response_code": "Received",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

