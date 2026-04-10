
# Page 1

*This model accepts additional fields of type Any.*

## Structure

`Page1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `number` | `int` | Optional | The current page number of the page to be retrieved.<br><br>**Constraints**: `>= 1` |
| `size` | `int` | Optional | The maximum number of records ta will be returned per page.<br><br>**Constraints**: `>= 1`, `<= 5000` |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "number": 1,
  "size": 50,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

