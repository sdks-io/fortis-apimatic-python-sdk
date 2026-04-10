
# Method 3

*This model accepts additional fields of type Any.*

## Structure

`Method3`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `mtype` | [`Type29`](../../doc/models/type-29.md) | Optional | - |
| `product_transaction_id` | `str` | Optional | The product_transaction_id of the cc or ach deposit account that the transaction is inteded for. Use only the cc or ach id to display their respective elements form only. The Product's method (cc/ach) has to match the type.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "type": "ach",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

