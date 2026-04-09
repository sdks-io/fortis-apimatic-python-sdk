
# Response Apple Pay Validate Merchant

## Structure

`ResponseApplePayValidateMerchant`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `mtype` | [`Type136Enum`](../../doc/models/type-136-enum.md) | Optional | Resource Type<br><br>**Default**: `"ApplePayValidateMerchant"` |
| `data` | [`Data37`](../../doc/models/data-37.md) | Optional | - |

## Example (as JSON)

```json
{
  "type": "ApplePayValidateMerchant",
  "data": {
    "merchantSession": "merchantSession0"
  }
}
```

