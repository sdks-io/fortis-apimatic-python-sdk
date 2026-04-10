
# Level 3 Default

Level3 Default

*This model accepts additional fields of type Any.*

## Structure

`Level3Default`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `destination_country_code` | `str` | Optional | Code of the country where the goods are being shipped.<br><br>**Constraints**: *Minimum Length*: `3`, *Maximum Length*: `3` |
| `duty_amount` | `int` | Optional | Fee amount associated with the import of the purchased goods ,Can accept Two (2) decimal places<br><br>**Constraints**: `>= 0`, `<= 99999999999900` |
| `freight_amount` | `int` | Optional | Freight or shipping portion of the total transaction amount ,Can accept Two (2) decimal places.<br><br>**Constraints**: `>= 0`, `<= 99999999999900` |
| `national_tax` | `int` | Optional | National tax for the transaction ,Can accept Two (2) decimal places.<br><br>**Constraints**: `<= 999999999900` |
| `sales_tax` | `int` | Optional | Sales tax for the transaction ,Can accept Two (2) decimal places.<br><br>**Constraints**: `<= 999999999900` |
| `shipfrom_zip_code` | `str` | Optional | Postal/ZIP code of the address from where the purchased goods are being shipped.<br><br>**Constraints**: *Maximum Length*: `10` |
| `shipto_zip_code` | `str` | Optional | Postal/ZIP code of the address where purchased goods will be delivered.<br><br>**Constraints**: *Maximum Length*: `10` |
| `tax_amount` | `int` | Optional | Amount of any value added taxes ,Can accept Two (2) decimal places.<br><br>**Constraints**: `>= 0`, `<= 99999999900` |
| `tax_exempt` | `Any` | Optional | - |
| `customer_vat_registration` | `str` | Optional | Customer VAT Registration<br><br>**Constraints**: *Maximum Length*: `13` |
| `merchant_vat_registration` | `str` | Optional | Merchant VAT Registration<br><br>**Constraints**: *Maximum Length*: `20` |
| `order_date` | `str` | Optional | Order Date<br><br>**Constraints**: *Minimum Length*: `6`, *Maximum Length*: `6` |
| `summary_commodity_code` | `str` | Optional | Summary Commodity Code<br><br>**Constraints**: *Maximum Length*: `4` |
| `tax_rate` | `int` | Optional | Tax rate used to calculate the sales tax amount, can accept 2 decimal places.<br><br>**Constraints**: `<= 999999` |
| `unique_vat_ref_number` | `str` | Optional | Unique VAT Reference Number<br><br>**Constraints**: *Maximum Length*: `15` |
| `line_items` | [`List[LineItem]`](../../doc/models/line-item.md) | Optional | Array of line items in transaction |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "destination_country_code": "840",
  "duty_amount": 0,
  "freight_amount": 0,
  "national_tax": 2,
  "sales_tax": 200,
  "shipfrom_zip_code": "AZ12345",
  "shipto_zip_code": "MI48335",
  "tax_amount": 0,
  "customer_vat_registration": "12345678",
  "merchant_vat_registration": "123456",
  "order_date": "171006",
  "summary_commodity_code": "C1K2",
  "tax_rate": 0,
  "unique_vat_ref_number": "vat1234",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

