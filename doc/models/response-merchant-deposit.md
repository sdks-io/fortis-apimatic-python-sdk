
# Response Merchant Deposit

## Structure

`ResponseMerchantDeposit`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `mtype` | [`Type47Enum`](../../doc/models/type-47-enum.md) | Optional | Resource Type<br><br>**Default**: `"MerchantDeposit"` |
| `data` | [`Data14`](../../doc/models/data-14.md) | Optional | - |

## Example (as JSON)

```json
{
  "type": "MerchantDeposit",
  "data": {
    "id": "id0",
    "company_id": "company_id6",
    "merchant_id": "merchant_id0",
    "service": "service0",
    "deposit_types": [
      "deposit",
      "adjustment",
      "fee"
    ]
  }
}
```

