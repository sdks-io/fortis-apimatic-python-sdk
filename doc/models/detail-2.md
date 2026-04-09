
# Detail 2

## Structure

`Detail2`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `processor_batch_number` | `str` | Optional | Processor Batch Number |
| `product_code` | `str` | Optional | Product Code |
| `deposit_detail_type` | `str` | Optional | Deposit Detail Type |
| `amount` | `float` | Optional | Amount |
| `memo` | `str` | Optional | Memo |
| `reported_date` | `str` | Optional | Reported Date<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` |
| `settled_date` | `str` | Optional | Settled Date<br><br>**Constraints**: *Maximum Length*: `10`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}$` |
| `mid` | `str` | Optional | Merchant ID |

## Example (as JSON)

```json
{
  "amount": 2487.24,
  "reported_date": "2021-12-01",
  "settled_date": "2021-12-01",
  "processor_batch_number": "processor_batch_number6",
  "product_code": "product_code8",
  "deposit_detail_type": "deposit_detail_type6",
  "memo": "memo6"
}
```

