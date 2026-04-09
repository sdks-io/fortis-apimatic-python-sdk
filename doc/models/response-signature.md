
# Response Signature

## Structure

`ResponseSignature`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `mtype` | [`Type72Enum`](../../doc/models/type-72-enum.md) | Optional | Resource Type<br><br>**Default**: `"Signature"` |
| `data` | [`Data21`](../../doc/models/data-21.md) | Optional | - |

## Example (as JSON)

```json
{
  "type": "Signature",
  "data": {
    "signature": "signature8",
    "resource": "AccountVault",
    "resource_id": "resource_id6",
    "id": "id0",
    "created_ts": 114
  }
}
```

