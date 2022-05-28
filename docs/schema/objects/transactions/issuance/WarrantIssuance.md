:house: [Documentation Home](/README.md)

---

### Object - Warrant Issuance Transaction

`https://opencaptablecoalition.com/schema/objects/transactions/issuance/WarrantIssuance.schema.json`

**Description:** _Object describing warrant issuance transaction by the issuer and held by a stakeholder_

**Data Type:** `OCF Object - TX_WARRANT_ISSUANCE`

**Composed From:**

- [schema/primitives/BaseObject](/docs/schema/primitives/BaseObject.md)
- [schema/primitives/transactions/BaseTransaction](/docs/schema/primitives/transactions/BaseTransaction.md)
- [schema/primitives/transactions/BaseSecurityTransaction](/docs/schema/primitives/transactions/BaseSecurityTransaction.md)
- [schema/primitives/transactions/issuance/BaseIssuance](/docs/schema/primitives/transactions/issuance/BaseIssuance.md)

**Properties:**

| Property                | Type                                                                                                             | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 | Required   |
| ----------------------- | ---------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- |
| id                      | `STRING`                                                                                                         | Identifier for the object                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | `REQUIRED` |
| comments                | [`STRING`]                                                                                                       | Unstructured text comments related to and stored for the object                                                                                                                                                                                                                                                                                                                                                                                                                                             | -          |
| object_type             | **Constant:** `TX_WARRANT_ISSUANCE`</br>_Defined in [schema/enums/ObjectType](/docs/schema/enums/ObjectType.md)_ | Object type field                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | `REQUIRED` |
| date                    | [schema/types/Date](/docs/schema/types/Date.md)                                                                  | Date on which the transaction occurred                                                                                                                                                                                                                                                                                                                                                                                                                                                                      | `REQUIRED` |
| security_id             | `STRING`                                                                                                         | Identifier for the security (stock, plan security, warrant, or convertible) by which it can be referenced by other transaction objects. Note that while this identifier is created with an issuance object, it should be different than the issuance object's `id` field which identifies the issuance transaction object itself. All future transactions on the security (e.g. acceptance, transfer, cancel, etc.) must reference this `security_id` to qualify which security the transaction applies to. | `REQUIRED` |
| custom_id               | `STRING`                                                                                                         | A custom ID for this security (e.g. CN-1.)                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | `REQUIRED` |
| stakeholder_id          | `STRING`                                                                                                         | Identifier for the stakeholder that holds legal title to this security                                                                                                                                                                                                                                                                                                                                                                                                                                      | `REQUIRED` |
| board_approval_date     | [schema/types/Date](/docs/schema/types/Date.md)                                                                  | Date of board approval for the security                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | `REQUIRED` |
| consideration           | [schema/types/Monetary](/docs/schema/types/Monetary.md)                                                          | Consideration for the security                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | `REQUIRED` |
| security_law_exemptions | [ [schema/types/SecurityExemption](/docs/schema/types/SecurityExemption.md) ]                                    | List of security law exemptions (and applicable jurisdictions) for this security                                                                                                                                                                                                                                                                                                                                                                                                                            | `REQUIRED` |
| quantity                | [schema/types/Numeric](/docs/schema/types/Numeric.md)                                                            | Quantity of shares the warrant is exercisable for                                                                                                                                                                                                                                                                                                                                                                                                                                                           | `REQUIRED` |
| exercise_price          | [schema/types/Monetary](/docs/schema/types/Monetary.md)                                                          | The exercise price of the warrant                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | `REQUIRED` |
| purchase_price          | [schema/types/Monetary](/docs/schema/types/Monetary.md)                                                          | Actual purchase price of the warrant (sum up purported value of all consideration, including in-kind)                                                                                                                                                                                                                                                                                                                                                                                                       | `REQUIRED` |
| exercise_triggers       | [ [schema/types/conversion_triggers/WarrantTrigger](/docs/schema/types/conversion_triggers/WarrantTrigger.md) ]  | In event the Warrant can convert due to trigger events (e.g. Maturity, Next Qualified Financing, Change of Control, at Election of Holder), what are the terms?                                                                                                                                                                                                                                                                                                                                             | `REQUIRED` |
| warrant_expiration_date | [schema/types/Date](/docs/schema/types/Date.md)                                                                  | What is expiration date of the warrant (if applicable)                                                                                                                                                                                                                                                                                                                                                                                                                                                      | -          |
| vesting_terms_id        | `STRING`                                                                                                         | Identifier of the VestingTerms to which this security is subject. If not present, security is fully vested on issuance.                                                                                                                                                                                                                                                                                                                                                                                     | -          |

**Source Code:** [schema/objects/transactions/issuance/WarrantIssuance](/schema/objects/transactions/issuance/WarrantIssuance.schema.json)

**Examples:**

```json
[
  {
    "object_type": "TX_WARRANT_ISSUANCE",
    "id": "test-warrant-issuance-minimal",
    "security_id": "test-security-id",
    "date": "2022-02-01",
    "custom_id": "S-1",
    "stakeholder_id": "stakeholder-id",
    "board_approval_date": "2022-02-01",
    "consideration": {
      "amount": "1.00",
      "currency": "USD"
    },
    "security_law_exemptions": [],
    "quantity": "1000",
    "exercise_price": {
      "amount": "1.00",
      "currency": "USD"
    },
    "purchase_price": {
      "amount": "1.00",
      "currency": "USD"
    },
    "exercise_triggers": [
      {
        "trigger_id": "WARRANT-1.TRIG.1",
        "nickname": "Exercisable Until Expiration",
        "trigger_description": "The warrant is exercisable on or before its date of expiration",
        "trigger_type": "ELECTIVE_ON_OR_BEFORE_DATE",
        "trigger_date": "2029-01-01",
        "conversion_right": {
          "conversion_mechanism": {
            "mechanism_type": "FIXED_AMOUNT_CONVERSION",
            "converts_to_quantity": "10000.00"
          },
          "converts_to_stock_class_id": "stock-class-id"
        }
      }
    ],
    "warrant_expiration_date": "2032-02-01"
  },
  {
    "object_type": "TX_WARRANT_ISSUANCE",
    "id": "test-warrant-issuance-full-fields",
    "security_id": "test-warrant-security-id",
    "date": "2022-02-01",
    "security_law_exemptions": [
      {
        "description": "Exemption",
        "jurisdiction": "US"
      }
    ],
    "board_approval_date": "2022-02-01",
    "stakeholder_id": "stakeholder-id",
    "consideration": {
      "amount": "1.00",
      "currency": "USD"
    },
    "custom_id": "S-1",
    "quantity": "1000",
    "exercise_triggers": [
      {
        "trigger_id": "WARRANT-1.TRIG.1",
        "nickname": "Exercisable Until Expiration",
        "trigger_description": "The warrant is exercisable on or before its date of expiration",
        "trigger_type": "ELECTIVE_ON_OR_BEFORE_DATE",
        "trigger_date": "2032-02-01",
        "conversion_right": {
          "conversion_mechanism": {
            "mechanism_type": "FIXED_AMOUNT_CONVERSION",
            "converts_to_quantity": "10000.00"
          },
          "converts_to_stock_class_id": "stock-class-id"
        }
      }
    ],
    "purchase_price": {
      "amount": "1.00",
      "currency": "USD"
    },
    "exercise_price": {
      "amount": "1.00",
      "currency": "USD"
    },
    "comments": [
      "Here is a comment",
      "Here is another comment"
    ],
    "vesting_terms_id": "4yr-1yr-cliff-schedule",
    "warrant_expiration_date": "2032-02-01"
  }
]
```

Copyright © 2022 Open Cap Table Coalition.