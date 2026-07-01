# Verzuimrapportage Arbodiensten - Verzekeraars

Verzuimstandaard Arbodiensten ↔ Verzekeraars, release 2026.

| | |
|---|---|
| Schema | [`xsd/VerzuimrapportageArbodienst-Verzekeraar.xsd`](../xsd/VerzuimrapportageArbodienst-Verzekeraar.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/VerzuimRapportageArbodienstVerzekeraar/2026` |
| Versie | 2026.0 |
| Elementen | 45 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`VerzuimRapportageArbodienstVerzekeraar`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** | Bericht algemeen | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` | Bericht, code | 1..1 | an..5 | 00704 |
| &emsp;&emsp;`VnrBrCd` | Versienummer bericht, code | 1..1 | an..5 | 00004 |
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
| &emsp;&emsp;`VestigingsnrHandelsregister` | Vestigingsnummer | 0..1 | n..12 |  |
| &emsp;&emsp;`IdWrkgvrArbdnst` | Identificatie werkgever bij arbodienst | 1..1 | an..40 |  |
| &emsp;&emsp;`AansltnrGeguitwlngArbdnst` | Aansluitnummer gegevensuitwisseling Arbodienst | 1..1 | an..70 |  |
| &emsp;&emsp;`IDWrkgvrVerzekeraar` | Identificatie werkgever bij verzekeraar | 0..1 | an..40 |  |
| &emsp;&emsp;`Lhnr` | Loonheffingennummer | 0..1 | an..12 |  |
| &emsp;&emsp;**`Wrknmr`** | Werknemer | 1..* | groep |  |
| &emsp;&emsp;&emsp;`IdWrknmr` | Identificatie werknemer | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;`IdWrknmrArbdnst` | Identificatie werknemer arbodienst | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`IdWrknmrVzkr` | Identificatie werknemer verzekeraar | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;**`Dnstvbnd`** | Dienstverband | 1..999 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`IdDnstvbnd` | Identificatie dienstverband | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`PersNr` | Personeelsnummer | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;**`Vrzm`** | Verzuim | 1..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`VrzmgvlId` | Verzuimgeval identificatie | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`DatEerstVrzmdg` | Datum eerste verzuimdag | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`DatEndVrzmBeg` | Datum einde verzuimbegeleiding | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`RdnEndVrzmBegeleidingCd` | Reden einde verzuimbegeleiding,code | 0..1 | an2 | 01, 02, 03, 04, 05, 06, 99 |
| &emsp;&emsp;&emsp;&emsp;&emsp;**`WrkHrvAdv`** | Werkhervattingsadvies | 0..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`VrwrkCd` | Verwerking, code | 1..1 | an2 | 01, 03, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`IdWrkHrvAdv` | Identificatie werkhervattingsadvies bij Arbodienst | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`DatWerkhervattingsadvies` | Datum werkhervattingsadvies | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;**`WrkHrvPer`** | Werkhervattingsperiode | 1..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`Ingdat` | Ingangsdatum | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`Enddat` | Einddatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`PercZiekConformWerkhervattingsadvies` | Percentage ziek conform werkhervattingsadvies | 1..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;**`Actie`** | Actie | 0..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`DatPoortwActie` | Datum Poortwachtactie | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`PoortwachteractieCd` | Poortwachteractie, code | 1..1 | an2 | 01, 02, 03, 04, 05, 06, 07, 08, 09 |
