# Enum - Day Count Type Schema

```txt
https://opencaptablecoalition.com/schema/enums/DayCountType.schema.json#/properties/day_count_convention
```

Enumeration of how the number of days are determined per period

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                                            |
| :------------------ | :--------- | :------------- | :---------------------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------------------------------------------------------------------ |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [ConvertibleIssuance.schema.json*](../../schema/objects/transactions/issuance/ConvertibleIssuance.schema.json "open original schema") |

## day_count_convention Type

`string` ([Enum - Day Count Type](convertibleissuance-properties-enum---day-count-type.md))

## day_count_convention Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value          | Explanation |
| :------------- | :---------- |
| `"ACTUAL_365"` |             |
| `"30_360"`     |             |