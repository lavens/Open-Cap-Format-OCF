# File - Vesting Schedules Schema

```txt
https://opencaptablecoalition.com/schema/files/vesting_schedules_file
```

JSON containing file type identifier and list of vesting schedules

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                     |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [VestingSchedulesFile.schema.json](../../schema/files/VestingSchedulesFile.schema.json "open original schema") |

## File - Vesting Schedules Type

`object` ([File - Vesting Schedules](vestingschedulesfile.md))

all of

*   [Untitled undefined type in File - Vesting Schedules](vestingschedulesfile-allof-0.md "check type definition")

# File - Vesting Schedules Properties

| Property                | Type          | Required | Nullable       | Defined by                                                                                                                                                             |
| :---------------------- | :------------ | :------- | :------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [items](#items)         | `array`       | Required | cannot be null | [File - Vesting Schedules](vestingschedulesfile-properties-items.md "https://opencaptablecoalition.com/schema/files/vesting_schedules_file#/properties/items")         |
| [file_type](#file_type) | Not specified | Required | cannot be null | [File - Vesting Schedules](vestingschedulesfile-properties-file_type.md "https://opencaptablecoalition.com/schema/files/vesting_schedules_file#/properties/file_type") |

## items



`items`

*   is required

*   Type: unknown\[]

*   cannot be null

*   defined in: [File - Vesting Schedules](vestingschedulesfile-properties-items.md "https://opencaptablecoalition.com/schema/files/vesting_schedules_file#/properties/items")

### items Type

unknown\[]

## file_type



`file_type`

*   is required

*   Type: unknown

*   cannot be null

*   defined in: [File - Vesting Schedules](vestingschedulesfile-properties-file_type.md "https://opencaptablecoalition.com/schema/files/vesting_schedules_file#/properties/file_type")

### file_type Type

unknown

### file_type Constraints

**constant**: the value of this property must be equal to:

```json
"OCF_VESTING_SCHEDULES_FILE"
```