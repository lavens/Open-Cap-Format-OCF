:house: [Documentation Home](../../../../../README.md)

---

### Object - Financing

`https://raw.githubusercontent.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/main/schema/objects/transactions/financing/Financing.schema.json`

**Description:** _Object describing a financing_

**Data Type:** `OCF Object - TX_FINANCING`

**Composed From:**

- [schema/primitives/objects/Object](../../../primitives/objects/Object.md)
- [schema/primitives/objects/transactions/Transaction](../../../primitives/objects/transactions/Transaction.md)

**Properties:**

| Property    | Type                                                                                                  | Description                                                     | Required   |
| ----------- | ----------------------------------------------------------------------------------------------------- | --------------------------------------------------------------- | ---------- |
| id          | `STRING`                                                                                              | Identifier for the object                                       | `REQUIRED` |
| comments    | [`STRING`]                                                                                            | Unstructured text comments related to and stored for the object | -          |
| object_type | **Constant:** `TX_FINANCING`</br>_Defined in [schema/enums/ObjectType](../../../enums/ObjectType.md)_ | Object type field                                               | `REQUIRED` |
| date        | [schema/types/Date](../../../types/Date.md)                                                           | Date on which the transaction occurred                          | `REQUIRED` |
| name        | [schema/types/Name](../../../types/Name.md)                                                           | Name for the financing                                          | `REQUIRED` |

**Source Code:** [schema/objects/transactions/financing/Financing](../../../../../../schema/objects/transactions/financing/Financing.schema.json)

Copyright © 2024 Open Cap Table Coalition.
