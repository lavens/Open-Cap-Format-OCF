# Type - Ratio Schema

```txt
https://opencaptablecoalition.com/schema/types/Ratio.schema.json#/properties/ratio
```

Type representation of a ratio as antecedent and consequent numeric values

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :-------------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [ConversionTrigger.schema.json*](../../schema/types/ConversionTrigger.schema.json "open original schema") |

## ratio Type

`object` ([Type - Ratio](conversiontrigger-properties-type---ratio.md))

# ratio Properties

| Property                  | Type     | Required | Nullable       | Defined by                                                                                                                                       |
| :------------------------ | :------- | :------- | :------------- | :----------------------------------------------------------------------------------------------------------------------------------------------- |
| [antecedent](#antecedent) | `string` | Required | cannot be null | [Type - Ratio](ratio-properties-type---numeric.md "https://opencaptablecoalition.com/schema/types/Numeric.schema.json#/properties/antecedent")   |
| [consequent](#consequent) | `string` | Required | cannot be null | [Type - Ratio](ratio-properties-type---numeric-1.md "https://opencaptablecoalition.com/schema/types/Numeric.schema.json#/properties/consequent") |

## antecedent

Fixed-point string representation of a number (up to 10 decimal places supported)

`antecedent`

*   is required

*   Type: `string` ([Type - Numeric](ratio-properties-type---numeric-1.md))

*   cannot be null

*   defined in: [Type - Ratio](ratio-properties-type---numeric-1.md "https://opencaptablecoalition.com/schema/types/Numeric.schema.json#/properties/antecedent")

### antecedent Type

`string` ([Type - Numeric](ratio-properties-type---numeric-1.md))

### antecedent Constraints

**pattern**: the string must match the following regular expression: 

```regexp
^[+-]?[0-9]+(\.[0-9]{1,10})?$
```

[try pattern](https://regexr.com/?expression=%5E%5B%2B-%5D%3F%5B0-9%5D%2B\(%5C.%5B0-9%5D%7B1%2C10%7D\)%3F%24 "try regular expression with regexr.com")

## consequent

Fixed-point string representation of a number (up to 10 decimal places supported)

`consequent`

*   is required

*   Type: `string` ([Type - Numeric](ratio-properties-type---numeric-1.md))

*   cannot be null

*   defined in: [Type - Ratio](ratio-properties-type---numeric-1.md "https://opencaptablecoalition.com/schema/types/Numeric.schema.json#/properties/consequent")

### consequent Type

`string` ([Type - Numeric](ratio-properties-type---numeric-1.md))

### consequent Constraints

**pattern**: the string must match the following regular expression: 

```regexp
^[+-]?[0-9]+(\.[0-9]{1,10})?$
```

[try pattern](https://regexr.com/?expression=%5E%5B%2B-%5D%3F%5B0-9%5D%2B\(%5C.%5B0-9%5D%7B1%2C10%7D\)%3F%24 "try regular expression with regexr.com")