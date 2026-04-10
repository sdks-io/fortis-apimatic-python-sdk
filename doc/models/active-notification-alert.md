
# Active Notification Alert

*This model accepts additional fields of type Any.*

## Structure

`ActiveNotificationAlert`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `location_id` | `str` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |
| `location_api_id` | `str` | Optional | Location Api ID |
| `date_start` | `str` | Optional | Date Start<br><br>**Constraints**: *Maximum Length*: `19`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}\s[\d]{2}:[\d]{2}:[\d]{2}$` |
| `date_end` | `str` | Optional | Date End<br><br>**Constraints**: *Maximum Length*: `19`, *Pattern*: `^[\d]{4}-[\d]{2}-[\d]{2}\s[\d]{2}:[\d]{2}:[\d]{2}$` |
| `user_location` | `bool` | Optional | User Location |
| `user_contact` | `bool` | Optional | User Contact |
| `include_children` | `bool` | Optional | Include Children |
| `alert_type` | `Any` | Optional | - |
| `alert_type_id` | `Any` | Optional | - |
| `description` | `str` | Optional | Description<br><br>**Constraints**: *Maximum Length*: `32` |
| `alert_message` | `str` | Optional | Alert Message |
| `id` | `str` | Optional | Notification Alert ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |
| `created_ts` | `int` | Optional | Created Time Stamp |
| `modified_ts` | `int` | Optional | Modified Time Stamp |
| `created_user_id` | `str` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |
| `modified_user_id` | `str` | Optional | Last User ID that updated the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "date_start": "2021-12-01 10:10:00",
  "date_end": "2021-12-01 10:10:00",
  "user_location": true,
  "user_contact": true,
  "include_children": true,
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "modified_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "modified_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "location_api_id": "location_api_id4",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

