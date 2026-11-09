# Helsestatusverdier for studiesøk - Forskningsstudier for deltakere v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Helsestatusverdier for studiesøk**

## ValueSet: Helsestatusverdier for studiesøk 

| | |
| :--- | :--- |
| *Official URL*:http://hl7.no/fhir/ig/studyfinder/ValueSet/studyfinder-health-status-values | *Version*:0.1.0 |
| Draft as of 2026-11-09 | *Computable Name*:StudyFinderHealthStatusVS |

 **References** 

* [Helsestatus for potensiell studiedeltaker](StructureDefinition-studyfinder-health-status-observation.md)

### Logical Definition (CLD)

 

### Expansion

-------

 Explanation of the columns that may appear on this page: 

| | |
| :--- | :--- |
| Level | A few code lists that FHIR defines are hierarchical - each code is assigned a level. In this scheme, some codes are under other codes, and imply that the code they are under also applies |
| System | The source of the definition of the code (when the value set draws in codes defined elsewhere) |
| Code | The code (used as the code in the resource instance) |
| Display | The display (used in the*display*element of a[Coding](http://hl7.org/fhir/R4/datatypes.html#Coding)). If there is no display, implementers should not simply display the code, but map the concept into their application |
| Definition | An explanation of the meaning of the concept |
| Comments | Additional notes about how to use the code |



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "studyfinder-health-status-values",
  "url" : "http://hl7.no/fhir/ig/studyfinder/ValueSet/studyfinder-health-status-values",
  "version" : "0.1.0",
  "name" : "StudyFinderHealthStatusVS",
  "title" : "Helsestatusverdier for studiesøk",
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
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "NO",
      "display" : "Norway"
    }]
  }],
  "compose" : {
    "include" : [{
      "system" : "http://hl7.no/fhir/ig/studyfinder/CodeSystem/studyfinder-health-status-codes",
      "concept" : [{
        "code" : "no-known-indications"
      },
      {
        "code" : "known-indications"
      },
      {
        "code" : "not-assessed"
      }]
    }]
  }
}

```
