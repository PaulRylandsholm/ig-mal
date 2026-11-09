# Organisasjon for forskningsstudie - Forskningsstudier for deltakere v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Organisasjon for forskningsstudie**

## Resource Profile: Organisasjon for forskningsstudie 

| | |
| :--- | :--- |
| *Official URL*:http://hl7.no/fhir/ig/studyfinder/StructureDefinition/studyfinder-organization | *Version*:0.1.0 |
| Draft as of 2026-11-09 | *Computable Name*:StudyFinderOrganization |

 
Sponsor, ansvarlig organisasjon eller organisasjon som er studiested. 

**Usages:**

* Refer to this Profile: [Fysisk studiested](StructureDefinition-studyfinder-location.md) and [Forskningsstudie for studiefinning](StructureDefinition-studyfinder-research-study.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/hl7.fhir.no.studyfinder|current/StructureDefinition/StructureDefinition-studyfinder-organization.json)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-studyfinder-organization.csv), [Excel](StructureDefinition-studyfinder-organization.xlsx), [Schematron](StructureDefinition-studyfinder-organization.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "studyfinder-organization",
  "url" : "http://hl7.no/fhir/ig/studyfinder/StructureDefinition/studyfinder-organization",
  "version" : "0.1.0",
  "name" : "StudyFinderOrganization",
  "title" : "Organisasjon for forskningsstudie",
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
  "description" : "Sponsor, ansvarlig organisasjon eller organisasjon som er studiested.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "NO",
      "display" : "Norway"
    }]
  }],
  "fhirVersion" : "4.0.1",
  "mapping" : [{
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
    "identity" : "servd",
    "uri" : "http://www.omg.org/spec/ServD/1.0/",
    "name" : "ServD"
  },
  {
    "identity" : "w5",
    "uri" : "http://hl7.org/fhir/fivews",
    "name" : "FiveWs Pattern Mapping"
  }],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Organization",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Organization",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "Organization",
      "path" : "Organization"
    },
    {
      "id" : "Organization.name",
      "path" : "Organization.name",
      "min" : 1,
      "mustSupport" : true
    },
    {
      "id" : "Organization.telecom",
      "path" : "Organization.telecom",
      "mustSupport" : true
    },
    {
      "id" : "Organization.address",
      "path" : "Organization.address",
      "mustSupport" : true
    }]
  }
}

```
