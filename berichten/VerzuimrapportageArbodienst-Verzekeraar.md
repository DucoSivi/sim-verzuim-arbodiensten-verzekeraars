# Verzuimrapportage Arbodiensten - Verzekeraars

Verzuimstandaard Arbodiensten ↔ Verzekeraars, release 2021.

| | |
|---|---|
| Schema | [`xsd/VerzuimrapportageArbodienst-Verzekeraar.xsd`](../xsd/VerzuimrapportageArbodienst-Verzekeraar.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/VerzuimRapportageArbodienstVerzekeraar/2021` |
| Versie | 2021.0 |
| Elementen | 90 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`VerzuimRapportageArbodienstVerzekeraar`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** | Bericht algemeen | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` | an..5 | 1..1 | an..5 | 00704 |
| &emsp;&emsp;`VnrBrCd` | an..5 | 1..1 | an..5 | 00002 |
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
| &emsp;&emsp;`VestigingsnrHandelsregister` | n..12 | 0..1 | n..12 |  |
| &emsp;&emsp;`IdWrkgvrArbdnst` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;`AansltnrGeguitwlngArbdnst` | an..70 | 1..1 | an..70 |  |
| &emsp;&emsp;`IDWrkgvrVerzekeraar` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;`Lhnr` | an..12 | 0..1 | an..12 |  |
| &emsp;&emsp;**`Wrknmr`** | Werknemer | 1..* | groep |  |
| &emsp;&emsp;&emsp;`VrwrkCd` | an2 | 1..1 | an2 | 04 |
| &emsp;&emsp;&emsp;`IngdatMut` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`SofiNr` | n..9 | 0..1 | n..9 |  |
| &emsp;&emsp;&emsp;`Gebdat` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`Overldat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`SignNm` | an..200 | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;`Voorl` | a..6 | 1..1 | an..6 |  |
| &emsp;&emsp;&emsp;`Voorv` | a..10 | 0..1 | an..10 |  |
| &emsp;&emsp;&emsp;`Roepnaam` | a..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`TitVNm` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`TitANm` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`NmvrkrCd` | an2 | 1..1 | an2 | 01, 02, 03, 04 |
| &emsp;&emsp;&emsp;`GslchtCd` | an1 | 1..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;`IdWrknmr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;`IdWrknmrOud` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`IdWrknmrArbdnst` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`IdWrknmrVzkr` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;**`Prtnr`** | Partner | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`VrwrkCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;`SignNm` | an..200 | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;&emsp;`Voorv` | a..10 | 0..1 | an..10 |  |
| &emsp;&emsp;&emsp;**`StrAdrNl`** | Straatadres nederland | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`SrtAdrsCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05, 06 |
| &emsp;&emsp;&emsp;&emsp;`SrtVrplgadrsCd` | an2 | 0..1 | an2 | 01, 02, 03, 99 |
| &emsp;&emsp;&emsp;&emsp;`NmVrpladrs` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Pc` | an6 | 1..1 | an6 |  |
| &emsp;&emsp;&emsp;&emsp;`Wnpl` | an..24 | 1..1 | an..24 |  |
| &emsp;&emsp;&emsp;&emsp;`StraatLang` | an..80 | 0..1 | an..80 |  |
| &emsp;&emsp;&emsp;&emsp;`Huisnr` | n..5 | 1..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`HuisToev` | an..4 | 0..1 | an..4 |  |
| &emsp;&emsp;&emsp;**`StrAdrBl`** | Straatadres buitenland | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`SrtAdrsCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05, 06 |
| &emsp;&emsp;&emsp;&emsp;`SrtVrplgadrsCd` | an2 | 0..1 | an2 | 01, 02, 03, 99 |
| &emsp;&emsp;&emsp;&emsp;`NmVrpladrs` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`LocomsBtl` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`PcBtl` | an..9 | 0..1 | an..9 |  |
| &emsp;&emsp;&emsp;&emsp;`WnplBtl` | an..24 | 1..1 | an..24 |  |
| &emsp;&emsp;&emsp;&emsp;`RegBtl` | an..24 | 0..1 | an..24 |  |
| &emsp;&emsp;&emsp;&emsp;`LandCd` | a2 | 1..1 | an2 |  |
| &emsp;&emsp;&emsp;&emsp;`Landnm` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`StraatLang` | an..80 | 0..1 | an..80 |  |
| &emsp;&emsp;&emsp;&emsp;`HuisnrBtl` | an..9 | 1..1 | an..9 |  |
| &emsp;&emsp;&emsp;**`Dnstvbnd`** | Dienstverband | 1..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`IdDnstvbnd` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`PersNr` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`CntrnrArbdnst` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;**`Vrzm`** | Verzuim | 1..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`VrwrkCd` | an2 | 1..1 | an2 | 02, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`VrzmgvlId` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`DatEerstVrzmdg` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`DatEndVrzmBeg` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`RdnEndVrzmBegeleidingCd` | an2 | 0..1 | an2 | 01, 02, 03, 04, 05, 06, 99 |
| &emsp;&emsp;&emsp;&emsp;&emsp;**`WrkHrvAdv`** | Werkhervattingsadvies | 0..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`VrwrkCd` | an2 | 1..1 | an2 | 01, 03, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`IdWrkHrvAdv` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`DatWerkhervattingsadvies` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;**`WrkHrvPer`** | Werkhervattingsperiode | 1..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`Ingdat` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`PercZiekConformWerkhervattingsadvies` | n..6,2 | 1..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;**`Actie`** | Actie | 0..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`DatPoortwActie` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`PoortwachteractieCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05, 06, 07, 08, 09 |
