# Legemiddelbruk for vurdering mot studiekriterier - Forskningsstudier for deltakere v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Legemiddelbruk for vurdering mot studiekriterier**

## Resource Profile: Legemiddelbruk for vurdering mot studiekriterier 

| | |
| :--- | :--- |
| *Official URL*:http://hl7.no/fhir/ig/studyfinder/StructureDefinition/studyfinder-medication-statement | *Version*:0.1.0 |
| Draft as of 2026-11-09 | *Computable Name*:StudyFinderMedicationStatement |

 
Legemiddelbruk som kan være relevant for inklusjons- eller eksklusjonskriterier. 

**Usages:**

* This Profile is not used by any profiles in this Specification

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/hl7.fhir.no.studyfinder|current/StructureDefinition/StructureDefinition-studyfinder-medication-statement.json)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-studyfinder-medication-statement.csv), [Excel](StructureDefinition-studyfinder-medication-statement.xlsx), [Schematron](StructureDefinition-studyfinder-medication-statement.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "studyfinder-medication-statement",
  "url" : "http://hl7.no/fhir/ig/studyfinder/StructureDefinition/studyfinder-medication-statement",
  "version" : "0.1.0",
  "name" : "StudyFinderMedicationStatement",
  "title" : "Legemiddelbruk for vurdering mot studiekriterier",
  "status" : "draft",
  "date" : "2026-11-09T14:07:54+00:00",
  "publisher" : "HL7 Norge",
  "contact" : [{
    "name" : "HL7 Norge",
    "telecom" : [{
      "system" : "url",
      "value" : "https://www.hl7.no"
    }]
  }],
  "description" : "Legemiddelbruk som kan være relevant for inklusjons- eller eksklusjonskriterier.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "NO",
      "display" : "Norway"
    }]
  }],
  "fhirVersion" : "4.0.1",
  "mapping" : [{
    "identity" : "workflow",
    "uri" : "http://hl7.org/fhir/workflow",
    "name" : "Workflow Pattern"
  },
  {
    "identity" : "rim",
    "uri" : "http://hl7.org/v3",
    "name" : "RIM Mapping"
  },
  {
    "identity" : "w5",
    "uri" : "http://hl7.org/fhir/fivews",
    "name" : "FiveWs Pattern Mapping"
  },
  {
    "identity" : "v2",
    "uri" : "http://hl7.org/v2",
    "name" : "HL7 v2 Mapping"
  }],
  "kind" : "resource",
  "abstract" : false,
  "type" : "MedicationStatement",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/MedicationStatement",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "MedicationStatement",
      "path" : "MedicationStatement"
    },
    {
      "id" : "MedicationStatement.status",
      "path" : "MedicationStatement.status",
      "mustSupport" : true
    },
    {
      "id" : "MedicationStatement.medication[x]",
      "path" : "MedicationStatement.medication[x]",
      "mustSupport" : true
    },
    {
      "id" : "MedicationStatement.subject",
      "path" : "MedicationStatement.subject",
      "type" : [{
        "code" : "Reference",
        "targetProfile" : ["http://hl7.no/fhir/ig/studyfinder/StructureDefinition/studyfinder-participant"]
      }],
      "mustSupport" : true
    }]
  }
}

```
