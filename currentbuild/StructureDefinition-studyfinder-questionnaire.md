# Spørreskjema for studiesøk - Forskningsstudier for deltakere v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Spørreskjema for studiesøk**

## Resource Profile: Spørreskjema for studiesøk 

| | |
| :--- | :--- |
| *Official URL*:http://hl7.no/fhir/ig/studyfinder/StructureDefinition/studyfinder-questionnaire | *Version*:0.1.0 |
| Draft as of 2026-11-09 | *Computable Name*:StudyFinderQuestionnaire |

 
Spørreskjema for strukturert innhenting av nødvendige opplysninger fra en person som leter etter studier. 

**Usages:**

* This Profile is not used by any profiles in this Specification

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/hl7.fhir.no.studyfinder|current/StructureDefinition/StructureDefinition-studyfinder-questionnaire.json)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-studyfinder-questionnaire.csv), [Excel](StructureDefinition-studyfinder-questionnaire.xlsx), [Schematron](StructureDefinition-studyfinder-questionnaire.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "studyfinder-questionnaire",
  "url" : "http://hl7.no/fhir/ig/studyfinder/StructureDefinition/studyfinder-questionnaire",
  "version" : "0.1.0",
  "name" : "StudyFinderQuestionnaire",
  "title" : "Spørreskjema for studiesøk",
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
  "description" : "Spørreskjema for strukturert innhenting av nødvendige opplysninger fra en person som leter etter studier.",
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
    "identity" : "objimpl",
    "uri" : "http://hl7.org/fhir/object-implementation",
    "name" : "Object Implementation Information"
  },
  {
    "identity" : "v2",
    "uri" : "http://hl7.org/v2",
    "name" : "HL7 v2 Mapping"
  }],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Questionnaire",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Questionnaire",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "Questionnaire",
      "path" : "Questionnaire"
    },
    {
      "id" : "Questionnaire.status",
      "path" : "Questionnaire.status",
      "mustSupport" : true
    },
    {
      "id" : "Questionnaire.item",
      "path" : "Questionnaire.item",
      "min" : 1,
      "mustSupport" : true
    }]
  }
}

```
