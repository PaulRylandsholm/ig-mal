# Helsestatus for studiesøk - Forskningsstudier for deltakere v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Helsestatus for studiesøk**

## CodeSystem: Helsestatus for studiesøk 

| | |
| :--- | :--- |
| *Official URL*:http://hl7.no/fhir/ig/studyfinder/CodeSystem/studyfinder-health-status-codes | *Version*:0.1.0 |
| Draft as of 2026-11-09 | *Computable Name*:StudyFinderHealthStatusCS |

 This Code system is referenced in the content logical definition of the following value sets: 

* [Helsestatusverdier for studiesøk](ValueSet-studyfinder-health-status-values.md)



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "studyfinder-health-status-codes",
  "url" : "http://hl7.no/fhir/ig/studyfinder/CodeSystem/studyfinder-health-status-codes",
  "version" : "0.1.0",
  "name" : "StudyFinderHealthStatusCS",
  "title" : "Helsestatus for studiesøk",
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
  "content" : "complete",
  "count" : 4,
  "concept" : [{
    "code" : "health-status",
    "display" : "Helsestatus"
  },
  {
    "code" : "no-known-indications",
    "display" : "Ingen kjente indikasjoner"
  },
  {
    "code" : "known-indications",
    "display" : "Kjente indikasjoner"
  },
  {
    "code" : "not-assessed",
    "display" : "Ikke vurdert"
  }]
}

```
