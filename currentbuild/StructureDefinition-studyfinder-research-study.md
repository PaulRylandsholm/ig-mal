# Forskningsstudie for studiefinning - Forskningsstudier for deltakere v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Forskningsstudie for studiefinning**

## Resource Profile: Forskningsstudie for studiefinning 

| | |
| :--- | :--- |
| *Official URL*:http://hl7.no/fhir/ig/studyfinder/StructureDefinition/studyfinder-research-study | *Version*:0.1.0 |
| Draft as of 2026-11-09 | *Computable Name*:StudyFinderResearchStudy |

 
Forskningsstudie som kan vises for personer som leter etter studier de kan være aktuelle for. 

**Usages:**

* This Profile is not used by any profiles in this Specification

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/hl7.fhir.no.studyfinder|current/StructureDefinition/StructureDefinition-studyfinder-research-study.json)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-studyfinder-research-study.csv), [Excel](StructureDefinition-studyfinder-research-study.xlsx), [Schematron](StructureDefinition-studyfinder-research-study.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "studyfinder-research-study",
  "url" : "http://hl7.no/fhir/ig/studyfinder/StructureDefinition/studyfinder-research-study",
  "version" : "0.1.0",
  "name" : "StudyFinderResearchStudy",
  "title" : "Forskningsstudie for studiefinning",
  "status" : "draft",
  "date" : "2026-11-09T12:54:59+00:00",
  "publisher" : "HL7 Norge",
  "contact" : [{
    "name" : "HL7 Norge",
    "telecom" : [{
      "system" : "url",
      "value" : "https://www.hl7.no"
    }]
  }],
  "description" : "Forskningsstudie som kan vises for personer som leter etter studier de kan være aktuelle for.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "NO",
      "display" : "Norway"
    }]
  }],
  "fhirVersion" : "4.0.1",
  "mapping" : [{
    "identity" : "BRIDG5.1",
    "uri" : "https://bridgmodel.nci.nih.gov",
    "name" : "BRIDG 5.1 Mapping"
  },
  {
    "identity" : "v2",
    "uri" : "http://hl7.org/v2",
    "name" : "HL7 v2 Mapping"
  },
  {
    "identity" : "rim",
    "uri" : "http://hl7.org/v3",
    "name" : "RIM Mapping"
  },
  {
    "identity" : "clinicaltrials-gov",
    "uri" : "http://clinicaltrials.gov",
    "name" : "ClinicalTrials.gov Mapping"
  },
  {
    "identity" : "w5",
    "uri" : "http://hl7.org/fhir/fivews",
    "name" : "FiveWs Pattern Mapping"
  }],
  "kind" : "resource",
  "abstract" : false,
  "type" : "ResearchStudy",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/ResearchStudy",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "ResearchStudy",
      "path" : "ResearchStudy"
    },
    {
      "id" : "ResearchStudy.title",
      "path" : "ResearchStudy.title",
      "min" : 1,
      "mustSupport" : true
    },
    {
      "id" : "ResearchStudy.status",
      "path" : "ResearchStudy.status",
      "mustSupport" : true
    },
    {
      "id" : "ResearchStudy.enrollment",
      "path" : "ResearchStudy.enrollment",
      "type" : [{
        "code" : "Reference",
        "targetProfile" : ["http://hl7.no/fhir/ig/studyfinder/StructureDefinition/studyfinder-study-population"]
      }],
      "mustSupport" : true
    },
    {
      "id" : "ResearchStudy.sponsor",
      "path" : "ResearchStudy.sponsor",
      "type" : [{
        "code" : "Reference",
        "targetProfile" : ["http://hl7.no/fhir/ig/studyfinder/StructureDefinition/studyfinder-organization"]
      }],
      "mustSupport" : true
    },
    {
      "id" : "ResearchStudy.site",
      "path" : "ResearchStudy.site",
      "type" : [{
        "code" : "Reference",
        "targetProfile" : ["http://hl7.no/fhir/ig/studyfinder/StructureDefinition/studyfinder-location"]
      }],
      "mustSupport" : true
    }]
  }
}

```
