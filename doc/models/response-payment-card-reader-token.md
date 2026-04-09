
# Response Payment Card Reader Token

## Structure

`ResponsePaymentCardReaderToken`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `mtype` | [`Type58Enum`](../../doc/models/type-58-enum.md) | Optional | Resource Type<br><br>**Default**: `"PaymentCardReaderToken"` |
| `data` | [`Data17`](../../doc/models/data-17.md) | Optional | - |

## Example (as JSON)

```json
{
  "type": "PaymentCardReaderToken",
  "data": {
    "token": "token4"
  }
}
```

