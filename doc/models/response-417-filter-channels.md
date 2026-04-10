
# Response 417 Filter Channels

*This model accepts additional fields of type Any.*

## Structure

`Response417FilterChannels`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `status_code` | `int` | Optional | Response code |
| `error` | `str` | Optional | Expectation Failed |
| `message` | `str` | Optional | Channel filters are not set for this project |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "statusCode": 417,
  "error": "Expectation Failed",
  "message": "Channel filters are not set for this project",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

