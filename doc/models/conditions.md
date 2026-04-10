
# Conditions

*This model accepts additional fields of type Any.*

## Structure

`Conditions`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `method` | [`Method`](../../doc/models/method.md) | Optional | - |
| `values` | [`Values`](../../doc/models/values.md) | Optional | - |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "method": "xor",
  "values": "account_vault_id",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

