
# Batch Risk Config 1

*This model accepts additional fields of type Any.*

## Structure

`BatchRiskConfig1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `blind_refund_total_count` | `int` | Optional | Blind Refund Total Count<br><br>**Constraints**: `>= 0`, `<= 999999999` |
| `blind_refund_max_amount` | `int` | Optional | Blind Refund Max Amount<br><br>**Constraints**: `>= 0`, `<= 999999999` |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "blind_refund_total_count": 66,
  "blind_refund_max_amount": 128,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

