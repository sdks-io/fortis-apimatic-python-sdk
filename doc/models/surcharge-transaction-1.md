
# Surcharge Transaction 1

*This model accepts additional fields of type Any.*

## Structure

`SurchargeTransaction1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `str` | Optional | ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |
| `model_name` | `str` | Optional | Model Name |
| `transaction_id` | `str` | Optional | Transaction ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |
| `surcharge_fee` | `int` | Optional | Surcharge Fee<br><br>**Constraints**: `>= 0` |
| `surcharge_rate` | `int` | Optional | Surcharge Rate<br><br>**Constraints**: `>= 0` |
| `surcharge_amount` | `int` | Optional | Surcharge Amount<br><br>**Constraints**: `>= 0` |
| `surcharge_transaction_min` | `int` | Optional | Surcharge Transaction Minimum<br><br>**Constraints**: `>= 0` |
| `surcharge_transaction_max` | `int` | Optional | Surcharge Transaction Maximum<br><br>**Constraints**: `>= 0` |
| `created` | `int` | Optional | Created |
| `modified` | `int` | Optional | Modified |
| `created_user_id` | `str` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |
| `modified_user_id` | `str` | Optional | Last User ID that updated the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "model_name": "Model Name",
  "transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "surcharge_fee": 0,
  "surcharge_rate": 0,
  "created": 1422040992,
  "modified": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "modified_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

