
# V1 Recurrings Skip Payment Request

*This model accepts additional fields of type Any.*

## Structure

`V1RecurringsSkipPaymentRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `skip_count` | `int` | Required | Skip Count<br><br>**Constraints**: `>= 1`, `<= 99` |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "skip_count": 7,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

