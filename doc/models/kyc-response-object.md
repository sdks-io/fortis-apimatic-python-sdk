
# Kyc Response Object

Array of KYC response objects.

*This model accepts additional fields of type Any.*

## Structure

`KycResponseObject`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `value` | `str` | Required | KYC object value. |
| `mtype` | `str` | Required | KYC oject type.<br><br>**Constraints**: *Maximum Length*: `32` |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "value": "KYC value.",
  "type": "KYC type",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

