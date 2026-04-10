
# V1 Wallet Provider Apple Pay Validate Merchant Request

*This model accepts additional fields of type Any.*

## Structure

`V1WalletProviderApplePayValidateMerchantRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `url` | `str` | Required | Url obtained in the ApplePay button click event. Apple's URL that needs to be called to validate merchant. |
| `merchant_id` | `str` | Required | Merchant ID |
| `domain_name` | `str` | Required | Domain Name |
| `display_name` | `str` | Required | Title |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "url": "https://apple-pay-gateway-cert.apple.com/paymentservices/startSession",
  "merchantId": "abc1234",
  "domainName": "website.domain.com",
  "displayName": "Sandwich Market",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

