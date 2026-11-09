# Målgruppe for forskningsstudie - Forskningsstudier for deltakere v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Målgruppe for forskningsstudie**

## Resource Profile: Målgruppe for forskningsstudie 

| | |
| :--- | :--- |
| *Official URL*:http://hl7.no/fhir/ig/studyfinder/StructureDefinition/studyfinder-study-population | *Version*:0.1.0 |
| Draft as of 2026-11-09 | *Computable Name*:StudyFinderStudyPopulation |

 
Definisjon av målgruppen og strukturerte inklusjons- og eksklusjonskriterier for en forskningsstudie. 

**Usages:**

* Refer to this Profile: [Forskningsstudie for studiefinning](StructureDefinition-studyfinder-research-study.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/hl7.fhir.no.studyfinder|current/StructureDefinition/StructureDefinition-studyfinder-study-population.json)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-studyfinder-study-population.csv), [Excel](StructureDefinition-studyfinder-study-population.xlsx), [Schematron](StructureDefinition-studyfinder-study-population.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "studyfinder-study-population",
  "url" : "http://hl7.no/fhir/ig/studyfinder/StructureDefinition/studyfinder-study-population",
  "version" : "0.1.0",
  "name" : "StudyFinderStudyPopulation",
  "title" : "Målgruppe for forskningsstudie",
  "status" : "draft",
  "date" : "2026-11-09T12:40:26+00:00",
  "publisher" : "HL7 Norge",
  "contact" : [{
    "name" : "HL7 Norge",
    "telecom" : [{
      "system" : "url",
      "value" : "https://www.hl7.no"
    }]
  }],
  "description" : "Definisjon av målgruppen og strukturerte inklusjons- og eksklusjonskriterier for en forskningsstudie.",
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
    "identity" : "w5",
    "uri" : "http://hl7.org/fhir/fivews",
    "name" : "FiveWs Pattern Mapping"
  }],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Group",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Group",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "Group",
      "path" : "Group"
    },
    {
      "id" : "Group.type",
      "path" : "Group.type",
      "patternCode" : "person"
    },
    {
      "id" : "Group.actual",
      "path" : "Group.actual",
      "patternBoolean" : false
    },
    {
      "id" : "Group.characteristic",
      "path" : "Group.characteristic",
      "min" : 1,
      "mustSupport" : true
    },
    {
      "id" : "Group.characteristic.code",
      "path" : "Group.characteristic.code",
      "mustSupport" : true
    },
    {
      "id" : "Group.characteristic.value[x]",
      "path" : "Group.characteristic.value[x]",
      "mustSupport" : true
    },
    {
      "id" : "Group.characteristic.exclude",
      "path" : "Group.characteristic.exclude",
      "mustSupport" : true
    }]
  }
}

```
