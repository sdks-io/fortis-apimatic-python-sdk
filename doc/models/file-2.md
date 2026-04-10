
# File 2

*This model accepts additional fields of type Any.*

## Structure

`File2`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `file_name` | `str` | Optional | The file name including the extension |
| `content` | `str` | Optional | File contents as a base64 encoded string |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "file_name": "file_name6",
  "content": "content6",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

