
# Balance

*This model accepts additional fields of type Any.*

## Structure

`Balance`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `amount_type` | `str` | Optional | The type of amount balance |
| `account_type` | `str` | Optional | The type of account balance |
| `amount` | `int` | Optional | The amount of balance |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "amount": 1000,
  "amount_type": "amount_type4",
  "account_type": "account_type6",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

