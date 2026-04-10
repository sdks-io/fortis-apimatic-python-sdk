
# Ui Prefs

Ui Prefs

*This model accepts additional fields of type Any.*

## Structure

`UiPrefs`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `entry_page` | `str` | Optional | Ui Prefs Entry Page |
| `page_size` | `int` | Optional | Ui Prefs Page Size<br><br>**Constraints**: `>= 0`, `<= 99` |
| `report_export_type` | `Any` | Optional | - |
| `process_method` | `Any` | Optional | - |
| `default_terminal` | `str` | Optional | Ui Prefs Default Termianl<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` |
| `additional_properties` | `Dict[str, Any]` | Optional | - |

## Example (as JSON)

```json
{
  "entry_page": "dashboard",
  "page_size": 2,
  "default_terminal": "11e95f8ec39de8fbdb0a4f1a",
  "report_export_type": {
    "key1": "val1",
    "key2": "val2"
  },
  "process_method": {
    "key1": "val1",
    "key2": "val2"
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

