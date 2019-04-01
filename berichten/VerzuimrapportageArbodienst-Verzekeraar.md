# Verzuimrapportage Arbodiensten - Verzekeraars

Verzuimstandaard Arbodiensten ↔ Verzekeraars, release 2019.

| | |
|---|---|
| Schema | [`xsd/VerzuimrapportageArbodienst-Verzekeraar.xsd`](../xsd/VerzuimrapportageArbodienst-Verzekeraar.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/VerzuimRapportageArbodienstVerzekeraar/2019` |
| Versie | 2019.1 |
| Elementen | 89 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`Message`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** |  | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` |  | 1..1 | an..5 | 00704 |
| &emsp;&emsp;`VnrBrCd` |  | 1..1 | an..5 | 00001 |
| &emsp;&emsp;`AandatBr` |  | 1..1 | datum |  |
| &emsp;&emsp;`AantijdBr` |  | 1..1 | tijd |  |
| &emsp;&emsp;`IdInzndr` |  | 1..1 | an..40 |  |
| &emsp;&emsp;`IdOntvngr` |  | 1..1 | an..40 |  |
| &emsp;&emsp;`Berrefnr` |  | 1..1 | an..512 |  |
| &emsp;&emsp;`TestJN` |  | 1..1 | an1 | J, N |
| &emsp;&emsp;`OntvngstbevJN` |  | 1..1 | an1 | J, N |
| &emsp;&emsp;`IngdatVerslagperiode` |  | 0..1 | datum |  |
| &emsp;&emsp;`EnddatVerslagperiode` |  | 0..1 | datum |  |
| &emsp;**`Wrkgvr`** |  | 1..* | groep |  |
| &emsp;&emsp;`HndlsnmOrg` |  | 1..1 | an..100 |  |
| &emsp;&emsp;`InschrijvingsnrKvK` |  | 0..1 | n..8 |  |
| &emsp;&emsp;`VestigingsnrHandelsregister` |  | 0..1 | n..12 |  |
| &emsp;&emsp;`IdWrkgvrArbdnst` |  | 1..1 | an..40 |  |
| &emsp;&emsp;`AansltnrGeguitwlngArbdnst` |  | 1..1 | an..70 |  |
| &emsp;&emsp;`IDWrkgvrVerzekeraar` |  | 0..1 | an..40 |  |
| &emsp;&emsp;`Lhnr` |  | 0..1 | an..12 |  |
| &emsp;&emsp;**`Wrknmr`** |  | 1..* | groep |  |
| &emsp;&emsp;&emsp;`VrwrkCd` |  | 1..1 | an2 | 04 |
| &emsp;&emsp;&emsp;`IngdatMut` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`SofiNr` |  | 1..1 | n..9 |  |
| &emsp;&emsp;&emsp;`Gebdat` |  | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`Overldat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`SignNm` |  | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;`Voorl` |  | 1..1 | an..6 |  |
| &emsp;&emsp;&emsp;`Voorv` |  | 0..1 | an..10 |  |
| &emsp;&emsp;&emsp;`Roepnaam` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`TitVNm` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`TitANm` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`NmvrkrCd` |  | 1..1 | an2 | 01, 02, 03, 04 |
| &emsp;&emsp;&emsp;`GslchtCd` |  | 1..1 | an1 | M, V |
| &emsp;&emsp;&emsp;`IdWrknmr` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`IdWrknmrOud` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`IdWrknmrArbdnst` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`IdWrknmrVzkr` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;**`Prtnr`** |  | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`VrwrkCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;`SignNm` |  | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;&emsp;`Voorv` |  | 0..1 | an..10 |  |
| &emsp;&emsp;&emsp;**`StrAdrNl`** |  | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`SrtAdrsCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05, 06 |
| &emsp;&emsp;&emsp;&emsp;`SrtVrplgadrsCd` |  | 0..1 | an2 | 01, 02, 03, 99 |
| &emsp;&emsp;&emsp;&emsp;`NmVrpladrs` |  | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Pc` |  | 1..1 | an6 |  |
| &emsp;&emsp;&emsp;&emsp;`Wnpl` |  | 1..1 | an..24 |  |
| &emsp;&emsp;&emsp;&emsp;`StraatLang` |  | 0..1 | an..80 |  |
| &emsp;&emsp;&emsp;&emsp;`Huisnr` |  | 1..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`HuisToev` |  | 0..1 | an..4 |  |
| &emsp;&emsp;&emsp;**`StrAdrBl`** |  | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`SrtAdrsCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05, 06 |
| &emsp;&emsp;&emsp;&emsp;`SrtVrplgadrsCd` |  | 0..1 | an2 | 01, 02, 03, 99 |
| &emsp;&emsp;&emsp;&emsp;`NmVrpladrs` |  | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`LocomsBtl` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`PcBtl` |  | 0..1 | an..9 |  |
| &emsp;&emsp;&emsp;&emsp;`WnplBtl` |  | 1..1 | an..24 |  |
| &emsp;&emsp;&emsp;&emsp;`RegBtl` |  | 0..1 | an..24 |  |
| &emsp;&emsp;&emsp;&emsp;`LandCd` |  | 1..1 | an2 |  |
| &emsp;&emsp;&emsp;&emsp;`Landnm` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`StraatLang` |  | 0..1 | an..80 |  |
| &emsp;&emsp;&emsp;&emsp;`HuisnrBtl` |  | 1..1 | an..9 |  |
| &emsp;&emsp;&emsp;**`Dnstvbnd`** |  | 1..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`IdDnstvbnd` |  | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`PersNr` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`CntrnrArbdnst` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;**`Vrzm`** |  | 1..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`VrwrkCd` |  | 1..1 | an2 | 02, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`VrzmgvlId` |  | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`DatEerstVrzmdg` |  | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`DatEndVrzmBeg` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`RdnEndVrzmBegeleidingCd` |  | 0..1 | an2 | 01, 02, 03, 04, 05, 06, 99 |
| &emsp;&emsp;&emsp;&emsp;&emsp;**`WrkHrvAdv`** |  | 0..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`VrwrkCd` |  | 1..1 | an2 | 01, 03, 05 |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`IdWrkHrvAdv` |  | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`DatWerkhervattingsadvies` |  | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;**`WrkHrvPer`** |  | 1..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`Ingdat` |  | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`Enddat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`PercZiekConformWerkhervattingsadvies` |  | 1..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;**`Actie`** |  | 0..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`DatPoortwActie` |  | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`PoortwachteractieCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05, 06, 07, 08, 09 |
