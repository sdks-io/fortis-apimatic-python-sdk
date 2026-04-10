
# Additional Amount

*This model accepts additional fields of type Any.*

## Structure

`AdditionalAmount`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `mtype` | `Any` | Optional | - |
| `amount` | `int` | Optional | The amount of additional amount. |
| `account_type` | `Any` | Optional | - |
| `currency` | `float` | Optional | Currency Code |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "amount": 10,
  "currency": 840.0,
  "type": {
    "key1": "val1",
    "key2": "val2"
  },
  "account_type": {
    "key1": "val1",
    "key2": "val2"
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

