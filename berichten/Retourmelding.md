# Retourmelding

Verzuimstandaard Arbodiensten ↔ Verzekeraars, release 2019.

| | |
|---|---|
| Schema | [`xsd/Retourmelding.xsd`](../xsd/Retourmelding.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/Retourmelding/2019` |
| Versie | 2019.1 |
| Elementen | 16 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`Message`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** |  | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` |  | 1..1 | an..5 | 99999 |
| &emsp;&emsp;`VnrBrCd` |  | 1..1 | an..5 | 00001 |
| &emsp;&emsp;`AandatBr` |  | 1..1 | datum |  |
| &emsp;&emsp;`AantijdBr` |  | 1..1 | tijd |  |
| &emsp;&emsp;`IdInzndr` |  | 1..1 | an..40 |  |
| &emsp;&emsp;`IdOntvngr` |  | 1..1 | an..40 |  |
| &emsp;&emsp;`Berrefnr` |  | 1..1 | an..512 |  |
| &emsp;&emsp;`BerrefnrIngzndnBer` |  | 1..1 | an..512 |  |
| &emsp;&emsp;`TestJN` |  | 1..1 | an1 | J, N |
| &emsp;&emsp;`OntvngstbevJN` |  | 1..1 | an1 | J, N |
| &emsp;&emsp;`SrtRetmldngCd` |  | 1..1 | an2 | 01, 02, 03, 04 |
| &emsp;**`Foutmldng`** |  | 0..* | groep |  |
| &emsp;&emsp;`SrtFoutCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05, 06, 99 |
| &emsp;&emsp;`Toelchtng` |  | 0..1 | an..512 |  |
