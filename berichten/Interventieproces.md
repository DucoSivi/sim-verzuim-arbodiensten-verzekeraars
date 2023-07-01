# Interventieproces

Verzuimstandaard Arbodiensten ↔ Verzekeraars, release 2023.

| | |
|---|---|
| Schema | [`xsd/Interventieproces.xsd`](../xsd/Interventieproces.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/Interventieproces/2023` |
| Versie | 2023.0 |
| Elementen | 42 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`Interventieproces`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** | Bericht algemeen | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` | an..5 | 1..1 | an..5 | 00801 |
| &emsp;&emsp;`VnrBrCd` | an..5 | 1..1 | an..5 | 00001 |
| &emsp;&emsp;`FunctieBrCd` | an2 | 1..1 | an2 | 05, 06 |
| &emsp;&emsp;`AandatBr` | an10 | 1..1 | datum |  |
| &emsp;&emsp;`AantijdBr` | an8 | 1..1 | tijd |  |
| &emsp;&emsp;`IdInzndr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;`GebrSwPakket` | an..35 | 1..1 | an..35 |  |
| &emsp;&emsp;`IdOntvngr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;`Berrefnr` | an..512 | 1..1 | an..512 |  |
| &emsp;&emsp;`TestJN` | a1 | 1..1 | an1 | J, N |
| &emsp;&emsp;`OntvngstbevJN` | a1 | 1..1 | an1 | J, N |
| &emsp;&emsp;`IngdatVerslagperiode` | an10 | 0..1 | datum |  |
| &emsp;&emsp;`EnddatVerslagperiode` | an10 | 0..1 | datum |  |
| &emsp;**`Wrkgvr`** | Werkgever | 1..* | groep |  |
| &emsp;&emsp;`HndlsnmOrg` | an..100 | 1..1 | an..100 |  |
| &emsp;&emsp;`InschrijvingsnrKvK` | n..8 | 0..1 | n..8 |  |
| &emsp;&emsp;`IdWrkgvrArbdnst` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;`AansltnrGeguitwlngArbdnst` | an..70 | 1..1 | an..70 |  |
| &emsp;&emsp;`IDWrkgvrVerzekeraar` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;`Lhnr` | an..12 | 0..1 | an..12 |  |
| &emsp;&emsp;`IndERDWGA` | a1 | 0..1 | an1 | J, N |
| &emsp;&emsp;`IndERDZW` | a1 | 0..1 | an1 | J, N |
| &emsp;&emsp;**`Wrknmr`** | Werknemer | 1..* | groep |  |
| &emsp;&emsp;&emsp;`IdWrknmr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;`IdWrknmrArbdnst` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`IdWrknmrVzkr` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;**`Dnstvbnd`** | Dienstverband | 1..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`IdDnstvbnd` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`PersNr` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`LnLbPh` | n..9,2 | 0..1 | n..9,2 |  |
| &emsp;&emsp;&emsp;&emsp;`LnSV` | n..9,2 | 0..1 | n..9,2 |  |
| &emsp;&emsp;&emsp;&emsp;**`Arbeidsrelatie`** | Arbeidsrelatie | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`IdArbeidsrelatie` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`PersNr` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;**`Vrzm`** | Verzuim | 1..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`VrzmgvlId` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`DatEerstVrzmdg` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`InloopJN` | a1 | 0..1 | an1 | J, N |
| &emsp;&emsp;&emsp;&emsp;&emsp;`UitloopJN` | a1 | 0..1 | an1 | J, N |
| &emsp;&emsp;&emsp;&emsp;&emsp;`InterventieJN` | a1 | 1..1 | an1 |  |
