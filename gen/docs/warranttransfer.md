# Object - Warrant Transfer Transaction Schema

```txt
Objects.Transactions.Transfer.WarrantTransfer.schema.json
```

Object describing a transfer or secondary sale of a warrant security

| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                                                   |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :--------------------------------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [WarrantTransfer.schema.json](../../schema/objects/transactions/transfer/WarrantTransfer.schema.json "open original schema") |

## Object - Warrant Transfer Transaction Type

`object` ([Object - Warrant Transfer Transaction](warranttransfer.md))

all of

*   all of

    *   all of

        *   [Object - BaseObject](issuer-allof-object---baseobject.md "check type definition")

# Object - Warrant Transfer Transaction Properties

| Property                                          | Type          | Required | Nullable       | Defined by                                                                                                                                                                                   |
| :------------------------------------------------ | :------------ | :------- | :------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [quantity](#quantity)                             | `object`      | Required | cannot be null | [Object - Warrant Transfer Transaction](stockplan-properties-type---numeric.md "Types.Numeric.schema.json#/properties/quantity")                                                             |
| [id](#id)                                         | Not specified | Optional | cannot be null | [Object - Warrant Transfer Transaction](warranttransfer-properties-id.md "Objects.Transactions.Transfer.WarrantTransfer.schema.json#/properties/id")                                         |
| [comments](#comments)                             | Not specified | Optional | cannot be null | [Object - Warrant Transfer Transaction](warranttransfer-properties-comments.md "Objects.Transactions.Transfer.WarrantTransfer.schema.json#/properties/comments")                             |
| [security_id](#security_id)                       | Not specified | Optional | cannot be null | [Object - Warrant Transfer Transaction](warranttransfer-properties-security_id.md "Objects.Transactions.Transfer.WarrantTransfer.schema.json#/properties/security_id")                       |
| [date](#date)                                     | Not specified | Optional | cannot be null | [Object - Warrant Transfer Transaction](warranttransfer-properties-date.md "Objects.Transactions.Transfer.WarrantTransfer.schema.json#/properties/date")                                     |
| [consideration](#consideration)                   | Not specified | Optional | cannot be null | [Object - Warrant Transfer Transaction](warranttransfer-properties-consideration.md "Objects.Transactions.Transfer.WarrantTransfer.schema.json#/properties/consideration")                   |
| [balance_security_id](#balance_security_id)       | Not specified | Optional | cannot be null | [Object - Warrant Transfer Transaction](warranttransfer-properties-balance_security_id.md "Objects.Transactions.Transfer.WarrantTransfer.schema.json#/properties/balance_security_id")       |
| [resulting_security_ids](#resulting_security_ids) | Not specified | Optional | cannot be null | [Object - Warrant Transfer Transaction](warranttransfer-properties-resulting_security_ids.md "Objects.Transactions.Transfer.WarrantTransfer.schema.json#/properties/resulting_security_ids") |

## quantity

Type representation of a number (up to 10 decimal places supported by the spec)

`quantity`

*   is required

*   Type: `object` ([Type - Numeric](stockplan-properties-type---numeric.md))

*   cannot be null

*   defined in: [Object - Warrant Transfer Transaction](stockplan-properties-type---numeric.md "Types.Numeric.schema.json#/properties/quantity")

### quantity Type

`object` ([Type - Numeric](stockplan-properties-type---numeric.md))

## id



`id`

*   is optional

*   Type: unknown

*   cannot be null

*   defined in: [Object - Warrant Transfer Transaction](warranttransfer-properties-id.md "Objects.Transactions.Transfer.WarrantTransfer.schema.json#/properties/id")

### id Type

unknown

## comments



`comments`

*   is optional

*   Type: unknown

*   cannot be null

*   defined in: [Object - Warrant Transfer Transaction](warranttransfer-properties-comments.md "Objects.Transactions.Transfer.WarrantTransfer.schema.json#/properties/comments")

### comments Type

unknown

## security_id



`security_id`

*   is optional

*   Type: unknown

*   cannot be null

*   defined in: [Object - Warrant Transfer Transaction](warranttransfer-properties-security_id.md "Objects.Transactions.Transfer.WarrantTransfer.schema.json#/properties/security_id")

### security_id Type

unknown

## date



`date`

*   is optional

*   Type: unknown

*   cannot be null

*   defined in: [Object - Warrant Transfer Transaction](warranttransfer-properties-date.md "Objects.Transactions.Transfer.WarrantTransfer.schema.json#/properties/date")

### date Type

unknown

## consideration



`consideration`

*   is optional

*   Type: unknown

*   cannot be null

*   defined in: [Object - Warrant Transfer Transaction](warranttransfer-properties-consideration.md "Objects.Transactions.Transfer.WarrantTransfer.schema.json#/properties/consideration")

### consideration Type

unknown

## balance_security_id



`balance_security_id`

*   is optional

*   Type: unknown

*   cannot be null

*   defined in: [Object - Warrant Transfer Transaction](warranttransfer-properties-balance_security_id.md "Objects.Transactions.Transfer.WarrantTransfer.schema.json#/properties/balance_security_id")

### balance_security_id Type

unknown

## resulting_security_ids



`resulting_security_ids`

*   is optional

*   Type: unknown

*   cannot be null

*   defined in: [Object - Warrant Transfer Transaction](warranttransfer-properties-resulting_security_ids.md "Objects.Transactions.Transfer.WarrantTransfer.schema.json#/properties/resulting_security_ids")

### resulting_security_ids Type

unknown