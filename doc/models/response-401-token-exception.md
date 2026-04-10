
# Response 401 Token Exception

*This model accepts additional fields of type Any.*

## Structure

`Response401TokenException`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `status_code` | `int` | Optional | Response code |
| `error` | `str` | Optional | Unauthorized |
| `message` | `str` | Optional | Invalid token |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "statusCode": 401,
  "error": "Unauthorized",
  "message": "Invalid token",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

