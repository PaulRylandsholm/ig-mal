# Artifacts Summary - Forskningsstudier for deltakere v0.1.0

* [**Table of Contents**](toc.md)
* **Artifacts Summary**

## Artifacts Summary

This page provides a list of the FHIR artifacts defined as part of this implementation guide.

### Structures: Resource Profiles 

These define constraints on FHIR resources for systems conforming to this implementation guide.

| | |
| :--- | :--- |
| [Forskningsstudie for studiefinning](StructureDefinition-studyfinder-research-study.md) | Forskningsstudie som kan vises for personer som leter etter studier de kan være aktuelle for. |
| [Fysisk studiested](StructureDefinition-studyfinder-location.md) | Fysisk studiested med adresse og eventuell geografisk posisjon. |
| [Helsestatus for potensiell studiedeltaker](StructureDefinition-studyfinder-health-status-observation.md) | Eksplisitt helsestatus, inkludert om personen oppgir at det ikke foreligger kjente indikasjoner. |
| [Helsetilstand for vurdering mot studiekriterier](StructureDefinition-studyfinder-condition.md) | Helsetilstand som kan være relevant for inklusjons- eller eksklusjonskriterier. |
| [Legemiddelbruk for vurdering mot studiekriterier](StructureDefinition-studyfinder-medication-statement.md) | Legemiddelbruk som kan være relevant for inklusjons- eller eksklusjonskriterier. |
| [Målgruppe for forskningsstudie](StructureDefinition-studyfinder-study-population.md) | Definisjon av målgruppen og strukturerte inklusjons- og eksklusjonskriterier for en forskningsstudie. |
| [Måling for vurdering mot studiekriterier](StructureDefinition-studyfinder-observation.md) | Måling eller klinisk observasjon som kan være relevant for studiekriterier. |
| [Organisasjon for forskningsstudie](StructureDefinition-studyfinder-organization.md) | Sponsor, ansvarlig organisasjon eller organisasjon som er studiested. |
| [Potensiell studiedeltaker](StructureDefinition-studyfinder-participant.md) | Personopplysninger som kan brukes ved en foreløpig vurdering mot studiekriterier. |
| [Spørreskjema for studiesøk](StructureDefinition-studyfinder-questionnaire.md) | Spørreskjema for strukturert innhenting av nødvendige opplysninger fra en person som leter etter studier. |
| [Svar på spørreskjema for studiesøk](StructureDefinition-studyfinder-questionnaire-response.md) | Strukturerte opplysninger fra en person som leter etter studier. |

### Terminology: Value Sets 

These define sets of codes used by systems conforming to this implementation guide.

| |
| :--- |
| [Helsestatusverdier for studiesøk](ValueSet-studyfinder-health-status-values.md) |

### Terminology: Code Systems 

These define new code systems used by systems conforming to this implementation guide.

| |
| :--- |
| [Helsestatus for studiesøk](CodeSystem-studyfinder-health-status-codes.md) |

