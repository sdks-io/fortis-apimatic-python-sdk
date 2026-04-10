
# V1 Webhooks Transaction Request 1

*This model accepts additional fields of type Any.*

## Structure

`V1WebhooksTransactionRequest1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `attempt_interval` | `int` | Optional | Number of seconds before another retry is submitted<br><br>**Default**: `300`<br><br>**Constraints**: `>= 300`, `<= 86400` |
| `basic_auth_username` | `str` | Optional | The Basic authorization username for the URL, if not supplied, the postback will be submitted without Basic authorization headers<br><br>> This is only expandable for response but settable in the POST/PUT request<br><br>**Constraints**: *Maximum Length*: `512` |
| `basic_auth_password` | `str` | Optional | The basic authorization password<br><br>> This is only expandable for response but settable in the POST/PUT request<br><br>**Constraints**: *Maximum Length*: `512` |
| `expands` | `str` | Optional | An option list of expanded data to send with base data. (i.e. set this field to “contact,account_vault” to get the contact an accountvault used to run a transaction.)<br><br>**Constraints**: *Maximum Length*: `512` |
| `format` | `Any` | Optional | - |
| `is_active` | `bool` | Optional | Flag to indicate whether configuration is active (in effect). |
| `location_id` | `str` | Optional | The location identifier of the resource you want to recieve postbacks from.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |
| `location_api_id` | `str` | Optional | Location Api ID |
| `on_create` | `bool` | Optional | To receive postbacks on the creation of a resource |
| `on_update` | `bool` | Optional | To receive postbacks on the updating of a resource |
| `on_delete` | `bool` | Optional | To receive postbacks when the record is deleted |
| `legacy` | `bool` | Optional | Prefer the legacy api format.<br><br>**Default**: `True` |
| `postback_config_id` | `str` | Optional | Postback Config ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |
| `product_transaction_id` | `str` | Optional | Required when using 'transaction' or 'transactionbatch' resource<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |
| `resource` | `Any` | Optional | - |
| `number_of_attempts` | `int` | Optional | Maximum number of attempts on failure<br><br>**Constraints**: `>= 1`, `<= 5` |
| `url` | `str` | Optional | The URL where the postback will be submitted<br><br>**Constraints**: *Maximum Length*: `512` |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "attempt_interval": 300,
  "basic_auth_username": "tester",
  "basic_auth_password": "Test@522",
  "expands": "changelogs,tags",
  "is_active": true,
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "on_create": true,
  "on_update": true,
  "on_delete": true,
  "legacy": true,
  "postback_config_id": "11e95f8ec39de8fbdb0a4f1a",
  "product_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "number_of_attempts": 1,
  "url": "https://127.0.0.1/receiver",
  "format": {
    "key1": "val1",
    "key2": "val2"
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

