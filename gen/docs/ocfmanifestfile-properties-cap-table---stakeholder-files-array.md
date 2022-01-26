# Cap Table - Stakeholder File(s) Array Schema

```txt
https://opencaptablecoalition.com/schema/files/ocf_manifest_file#/properties/stakeholders_files
```

List of files containing lists of issuer stakeholders, indexed from the file containing the first such object created to the file containing the last (See separate /schema/files/stakeholders_file schema to validate loaded files)

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                            |
| :------------------ | :--------- | :------------- | :---------------------- | :---------------- | :-------------------- | :------------------ | :---------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [OCFManifestFile.schema.json*](../../schema/files/OCFManifestFile.schema.json "open original schema") |

## stakeholders_files Type

unknown\[]

## stakeholders_files Constraints

**minimum number of items**: the minimum number of items for this array is: `1`