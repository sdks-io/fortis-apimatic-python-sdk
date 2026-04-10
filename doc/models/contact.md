
# Contact

The Contact.

*This model accepts additional fields of type Any.*

## Structure

`Contact`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `first_name` | `str` | Optional | Contact's first name.<br><br>**Constraints**: *Maximum Length*: `20` |
| `last_name` | `str` | Optional | Contact's last name.<br><br>**Constraints**: *Maximum Length*: `20` |
| `email` | `str` | Optional | Contact's email address.<br><br>**Constraints**: *Maximum Length*: `100` |
| `phone_number` | `str` | Optional | Contact's phone.<br><br>**Constraints**: *Maximum Length*: `20` |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "first_name": "Jeffery",
  "last_name": "Todd",
  "email": "jtodd@example.com",
  "phone_number": "555-555-3456",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

