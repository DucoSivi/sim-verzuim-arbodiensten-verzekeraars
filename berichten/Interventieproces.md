# Interventieproces

Verzuimstandaard Arbodiensten ↔ Verzekeraars, release 2025.

| | |
|---|---|
| Schema | [`xsd/Interventieproces.xsd`](../xsd/Interventieproces.xsd) |
| Namespace | `http://www.ec-design.nl/SIVI/SDM/0.2/structures/Interventieproces2025` |
| Versie | . |
| Elementen | 42 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`Message`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** | Bericht algemeen | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` | Bericht, code | 1..1 | an..5 | 00801 |
| &emsp;&emsp;`VnrBrCd` | Versienummer bericht, code | 1..1 | an..5 | 00001 |
| &emsp;&emsp;`FunctieBrCd` | Functie bericht, code | 1..1 | an2 | 05, 06 |
| &emsp;&emsp;`AandatBr` | Aanmaakdatum bericht | 1..1 | datum |  |
| &emsp;&emsp;`AantijdBr` | Aanmaaktijd bericht | 1..1 | tijd |  |
| &emsp;&emsp;`IdInzndr` | Identificatie inzender | 1..1 | an..40 |  |
| &emsp;&emsp;`GebrSwPakket` | Gebruikt softwarepakket | 1..1 | an..35 |  |
| &emsp;&emsp;`IdOntvngr` | Identificatie ontvanger | 1..1 | an..40 |  |
| &emsp;&emsp;`Berrefnr` | Berichtreferentienummer | 1..1 | an..512 |  |
| &emsp;&emsp;`TestJN` | Test J/N | 1..1 | an1 | J, N |
| &emsp;&emsp;`OntvngstbevJN` | Ontvangstbevestiging gewenst J/N | 1..1 | an1 | J, N |
| &emsp;&emsp;`IngdatVerslagperiode` | Ingangsdatum Verslagperiode | 0..1 | datum |  |
| &emsp;&emsp;`EnddatVerslagperiode` | Einddatum verslagperiode | 0..1 | datum |  |
| &emsp;**`Wrkgvr`** | Werkgever | 1..* | groep |  |
| &emsp;&emsp;`HndlsnmOrg` | Handelsnaam organisatie | 1..1 | an..100 |  |
| &emsp;&emsp;`InschrijvingsnrKvK` | Inschrijvingsnummer Kamer van Koophandel | 0..1 | n..8 |  |
| &emsp;&emsp;`IdWrkgvrArbdnst` | Identificatie werkgever bij arbodienst | 1..1 | an..40 |  |
| &emsp;&emsp;`AansltnrGeguitwlngArbdnst` | Aansluitnummer gegevensuitwisseling Arbodienst | 1..1 | an..70 |  |
| &emsp;&emsp;`IDWrkgvrVerzekeraar` | Identificatie werkgever bij verzekeraar | 0..1 | an..40 |  |
| &emsp;&emsp;`Lhnr` | Loonheffingennummer | 0..1 | an..12 |  |
| &emsp;&emsp;`IndERDWGA` | Indicatie eigenrisicodrager voor de WGA | 0..1 | an1 | J, N |
| &emsp;&emsp;`IndERDZW` | Indicatie eigenrisicodrager voor de ZW | 0..1 | an1 | J, N |
| &emsp;&emsp;**`Wrknmr`** | Werknemer | 1..* | groep |  |
| &emsp;&emsp;&emsp;`IdWrknmr` | Identificatie werknemer | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;`IdWrknmrArbdnst` | Identificatie werknemer arbodienst | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`IdWrknmrVzkr` | Identificatie werknemer verzekeraar | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;**`Dnstvbnd`** | Dienstverband | 1..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`IdDnstvbnd` | Identificatie dienstverband | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`PersNr` | Personeelsnummer | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`LnLbPh` | Loon LB/PH | 0..1 | n..9,2 |  |
| &emsp;&emsp;&emsp;&emsp;`LnSV` | Loon SV | 0..1 | n..9,2 |  |
| &emsp;&emsp;&emsp;&emsp;**`Arbeidsrelatie`** | Arbeidsrelatie | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`IdArbeidsrelatie` | Identificatie arbeidsrelatie | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`PersNr` | Personeelsnummer | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;**`Vrzm`** | Verzuim | 1..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`VrzmgvlId` | Verzuimgeval identificatie | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`DatEerstVrzmdg` | Datum eerste verzuimdag | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`InloopJN` | Inloop J/N | 0..1 | an1 | J, N |
| &emsp;&emsp;&emsp;&emsp;&emsp;`UitloopJN` | Uitloop J/N | 0..1 | an1 | J, N |
| &emsp;&emsp;&emsp;&emsp;&emsp;`InterventieJN` | Interventie J/N | 1..1 | an1 |  |
