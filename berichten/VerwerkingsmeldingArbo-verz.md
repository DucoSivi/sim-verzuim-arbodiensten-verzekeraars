# Verwerkingsmelding arbodienst - verzekeraar

Verzuimstandaard Arbodiensten ↔ Verzekeraars, release 2025.

| | |
|---|---|
| Schema | [`xsd/VerwerkingsmeldingArbo-verz.xsd`](../xsd/VerwerkingsmeldingArbo-verz.xsd) |
| Namespace | `http://www.ec-design.nl/SIVI/SDM/0.2/structures/VerwerkingsmeldingArbo-verz2` |
| Versie | 00.00 |
| Elementen | 24 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`Message`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** | Bericht algemeen | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` | Bericht, code | 1..1 | an..5 | 00901 |
| &emsp;&emsp;`VnrBrCd` | Versienummer bericht, code | 1..1 | an..5 | 00001 |
| &emsp;&emsp;`AandatBr` | Aanmaakdatum bericht | 1..1 | datum |  |
| &emsp;&emsp;`AantijdBr` | Aanmaaktijd bericht | 1..1 | tijd |  |
| &emsp;&emsp;`IdInzndr` | Identificatie inzender | 1..1 | an..40 |  |
| &emsp;&emsp;`GebrSwPakket` | Gebruikt softwarepakket | 1..1 | an..35 |  |
| &emsp;&emsp;`IdOntvngr` | Identificatie ontvanger | 1..1 | an..40 |  |
| &emsp;&emsp;`Berrefnr` | Berichtreferentienummer | 1..1 | an..512 |  |
| &emsp;&emsp;`BerrefnrIngzndnBer` | Berichtreferentienummer ingezonden bericht | 1..1 | an..512 |  |
| &emsp;&emsp;`TestJN` | Test J/N | 1..1 | an1 | J, N |
| &emsp;&emsp;`OntvngstbevJN` | Ontvangstbevestiging gewenst J/N | 1..1 | an1 | J, N |
| &emsp;**`VrwrkMld`** | Verwerkingsmelding | 1..* | groep |  |
| &emsp;&emsp;`VrwrkbhdCd` | Verwerkbaarheid, code | 1..1 | an2 | 01, 02, 03 |
| &emsp;&emsp;`VrzmgvlId` | Verzuimgeval identificatie | 1..1 | an..40 |  |
| &emsp;&emsp;`VrzmgvlVnrMld` | Verzuimgeval volgnummer melding | 1..1 | n..3 |  |
| &emsp;&emsp;`AansltnrGeguitwlngArbdnst` | Aansluitnummer gegevensuitwisseling Arbodienst | 1..1 | an..70 |  |
| &emsp;&emsp;`IdWrkgvrArbdnst` | Identificatie werkgever bij arbodienst | 1..1 | an..40 |  |
| &emsp;&emsp;`IDWrkgvrVerzekeraar` | Identificatie werkgever bij verzekeraar | 1..1 | an..40 |  |
| &emsp;&emsp;`CtrlCd` | Controle, code | 1..1 | an5 |  |
| &emsp;&emsp;`MldngTkst` | Meldingstekst | 1..1 | an..512 |  |
| &emsp;&emsp;**`VrTkst`** | Vrije tekst | 0..1 | groep |  |
| &emsp;&emsp;&emsp;`VrijeTekst` | Vrije tekst | 1..1 | an..512 |  |
