
# List 8

*This model accepts additional fields of type Any.*

## Structure

`List8`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `str` | Optional | Deposit Id |
| `company_id` | `str` | Optional | Company Id |
| `merchant_id` | `str` | Optional | Merchant Id |
| `service` | `str` | Optional | Service |
| `deposit_types` | [`List[DepositType]`](../../doc/models/deposit-type.md) | Optional | - |
| `deposit_amount` | `float` | Optional | Deposit Amount |
| `batch_amount` | `float` | Optional | Batch Amount |
| `adjustment_amount` | `float` | Optional | Adjustment Amount |
| `retained_amount` | `float` | Optional | Retained Amount |
| `conveyed_amount` | `float` | Optional | Conveyed Amount |
| `fee_amount` | `float` | Optional | Fee Amount |
| `reference_number` | `str` | Optional | Reference Number |
| `trace_number` | `str` | Optional | - |
| `currency` | `str` | Optional | Currency |
| `created_ts` | `int` | Optional | Created Timestamp |
| `reported_date` | `str` | Optional | Reported Date<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` |
| `transaction_date` | `str` | Optional | Transaction Date<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` |
| `deposit_account` | `str` | Optional | Deposit Account |
| `details` | [`List[Detail2]`](../../doc/models/detail-2.md) | Optional | - |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "company_id": "8410111",
  "merchant_id": "88441",
  "deposit_amount": 2487.24,
  "batch_amount": 2487.24,
  "adjustment_amount": 2487.24,
  "retained_amount": 2487.24,
  "conveyed_amount": 2487.24,
  "fee_amount": 2487.24,
  "reference_number": "400000",
  "trace_number": "400000",
  "currency": "USD",
  "created_ts": 1422040992,
  "reported_date": "2021-12-01",
  "transaction_date": "2021-12-01",
  "id": "id0",
  "service": "service0",
  "deposit_types": [
    "fee",
    "deposit"
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

