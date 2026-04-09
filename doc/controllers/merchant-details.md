# Merchant Details

```python
merchant_details_controller = client.merchant_details
```

## Class Name

`MerchantDetailsController`


# Merchant Details

Merchant Details

```python
def merchant_details(self,
                    body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`V1WalletProviderMerchantDetailsRequest`](../../doc/models/v1-wallet-provider-merchant-details-request.md) | Body, Required | - |

## Response Type

[`ResponseMerchantDetails`](../../doc/models/response-merchant-details.md)

## Example Usage

```python
body = V1WalletProviderMerchantDetailsRequest(
    merchant_origin='dev.pay.site'
)

result = merchant_details_controller.merchant_details(body)
print(result)
```

## Example Response *(as JSON)*

```json
{
  "type": "MerchantDetails",
  "data": {
    "resultCode": false,
    "merchantID": "abc1234",
    "applePay": true,
    "googlePay": true,
    "applePayDomains": [
      null
    ],
    "message": "valid user",
    "googleJWT": "45r8v29bvj4gc904jfd932nm"
  }
}
```

## Errors

| HTTP Status Code | Error Description | Exception Class |
|  --- | --- | --- |
| 401 | Unauthorized | [`Response401tokenException`](../../doc/models/response-401-token-exception.md) |
| 412 | Precondition Failed | [`Response412Exception`](../../doc/models/response-412-exception.md) |

