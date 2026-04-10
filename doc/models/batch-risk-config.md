
# Batch Risk Config

Batch Risk Config

*This model accepts additional fields of type Any.*

## Structure

`BatchRiskConfig`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `blind_refund_total_count` | `int` | Optional | Blind Refund Total Count<br><br>**Constraints**: `>= 0`, `<= 999999999` |
| `blind_refund_max_amount` | `int` | Optional | Blind Refund Max Amount<br><br>**Constraints**: `>= 0`, `<= 999999999` |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "blind_refund_total_count": 110,
  "blind_refund_max_amount": 172,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

