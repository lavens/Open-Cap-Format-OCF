:house: [Documentation Home](../../../README.md)

---

### Object - Financing

`https://raw.githubusercontent.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/main/schema/objects/Financing.schema.json`

**Description:** _Object describing a financing_

**Data Type:** `OCF Object - FINANCING`

**Composed From:**

- [schema/primitives/objects/Object](../primitives/objects/Object.md)

**Properties:**

| Property    | Type                                                                                         | Description                                                     | Required   |
| ----------- | -------------------------------------------------------------------------------------------- | --------------------------------------------------------------- | ---------- |
| id          | `STRING`                                                                                     | Identifier for the object                                       | `REQUIRED` |
| comments    | [`STRING`]                                                                                   | Unstructured text comments related to and stored for the object | -          |
| object_type | **Constant:** `FINANCING`</br>_Defined in [schema/enums/ObjectType](../enums/ObjectType.md)_ | Object type field                                               | `REQUIRED` |
| name        | `STRING`                                                                                     | Name for the financing                                          | `REQUIRED` |

**Source Code:** [schema/objects/Financing](../../../../schema/objects/Financing.schema.json)

Copyright © 2024 Open Cap Table Coalition.
