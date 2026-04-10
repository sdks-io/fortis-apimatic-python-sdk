
# Alt Bank Account 2

*This model accepts additional fields of type Any.*

## Structure

`AltBankAccount2`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `routing_number` | `str` | Optional | Nine-digit Bank routing number.<br><br>**Constraints**: *Maximum Length*: `9` |
| `account_number` | `str` | Optional | Bank account number.<br><br>**Constraints**: *Maximum Length*: `17` |
| `account_holder_name` | `str` | Optional | Name on bank account.<br><br>**Constraints**: *Maximum Length*: `40` |
| `deposit_type` | `str` | Optional | Deposit type. |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "routing_number": "011103093",
  "account_number": "01234567890123",
  "account_holder_name": "Bob Fairview",
  "deposit_type": "fees_adjustments",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

