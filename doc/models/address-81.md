
# Address 81

Array of merchant addresses.

*This model accepts additional fields of type Any.*

## Structure

`Address81`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `address_line_1` | `str` | Required | Line 1 of address.<br><br>**Constraints**: *Maximum Length*: `100` |
| `address_line_2` | `str` | Optional | Line 2 of address.<br><br>**Constraints**: *Maximum Length*: `20` |
| `city` | `str` | Required | City of address.<br><br>**Constraints**: *Maximum Length*: `50` |
| `state_province` | `str` | Required | State or province of address.<br><br>**Constraints**: *Maximum Length*: `2` |
| `postal_code` | `str` | Required | Postal code of address.<br><br>**Constraints**: *Maximum Length*: `10` |
| `country_code` | `str` | Required | Country of address.<br><br>**Constraints**: *Maximum Length*: `2` |
| `address_type` | [`AddressType`](../../doc/models/address-type.md) | Required | **Constraints**: *Maximum Length*: `20` |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "address_line_1": "121 E Main",
  "address_line_2": "Apt 707",
  "city": "Dallas",
  "state_province": "TX",
  "postal_code": "75087",
  "country_code": "US",
  "address_type": "corporate",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

