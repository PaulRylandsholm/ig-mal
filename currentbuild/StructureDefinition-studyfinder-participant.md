# Potensiell studiedeltaker - Forskningsstudier for deltakere v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Potensiell studiedeltaker**

## Resource Profile: Potensiell studiedeltaker 

| | |
| :--- | :--- |
| *Official URL*:http://hl7.no/fhir/ig/studyfinder/StructureDefinition/studyfinder-participant | *Version*:0.1.0 |
| Draft as of 2026-11-09 | *Computable Name*:StudyFinderParticipant |

 
Personopplysninger som kan brukes ved en foreløpig vurdering mot studiekriterier. 

**Usages:**

* Refer to this Profile: [Helsetilstand for vurdering mot studiekriterier](StructureDefinition-studyfinder-condition.md), [Helsestatus for potensiell studiedeltaker](StructureDefinition-studyfinder-health-status-observation.md), [Legemiddelbruk for vurdering mot studiekriterier](StructureDefinition-studyfinder-medication-statement.md), [Måling for vurdering mot studiekriterier](StructureDefinition-studyfinder-observation.md) and [Svar på spørreskjema for studiesøk](StructureDefinition-studyfinder-questionnaire-response.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/hl7.fhir.no.studyfinder|current/StructureDefinition/StructureDefinition-studyfinder-participant.json)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-studyfinder-participant.csv), [Excel](StructureDefinition-studyfinder-participant.xlsx), [Schematron](StructureDefinition-studyfinder-participant.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "studyfinder-participant",
  "url" : "http://hl7.no/fhir/ig/studyfinder/StructureDefinition/studyfinder-participant",
  "version" : "0.1.0",
  "name" : "StudyFinderParticipant",
  "title" : "Potensiell studiedeltaker",
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
  "description" : "Personopplysninger som kan brukes ved en foreløpig vurdering mot studiekriterier.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "NO",
      "display" : "Norway"
    }]
  }],
  "fhirVersion" : "4.0.1",
  "mapping" : [{
    "identity" : "rim",
    "uri" : "http://hl7.org/v3",
    "name" : "RIM Mapping"
  },
  {
    "identity" : "cda",
    "uri" : "http://hl7.org/v3/cda",
    "name" : "CDA (R2)"
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
  },
  {
    "identity" : "loinc",
    "uri" : "http://loinc.org",
    "name" : "LOINC code for the element"
  }],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Patient",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Patient",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "Patient",
      "path" : "Patient"
    },
    {
      "id" : "Patient.gender",
      "path" : "Patient.gender",
      "mustSupport" : true
    },
    {
      "id" : "Patient.birthDate",
      "path" : "Patient.birthDate",
      "mustSupport" : true
    },
    {
      "id" : "Patient.address",
      "path" : "Patient.address",
      "mustSupport" : true
    },
    {
      "id" : "Patient.address.city",
      "path" : "Patient.address.city",
      "mustSupport" : true
    },
    {
      "id" : "Patient.address.postalCode",
      "path" : "Patient.address.postalCode",
      "mustSupport" : true
    }]
  }
}

```
