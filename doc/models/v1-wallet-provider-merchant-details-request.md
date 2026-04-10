
# V1 Wallet Provider Merchant Details Request

*This model accepts additional fields of type Any.*

## Structure

`V1WalletProviderMerchantDetailsRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `merchant_origin` | `str` | Required | Domain name where the Apple or Google pay button is or will be displayed. Full domain name including subdomain. |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "merchantOrigin": "dev.pay.site",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

