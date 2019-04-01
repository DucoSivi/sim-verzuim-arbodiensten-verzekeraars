# Verzuimmelding Verzekeraars - Arbodiensten

Verzuimstandaard Arbodiensten ↔ Verzekeraars, release 2019.

| | |
|---|---|
| Schema | [`xsd/VerzuimmeldingenVerzekeraar-Arbodienst.xsd`](../xsd/VerzuimmeldingenVerzekeraar-Arbodienst.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/VerzuimmeldingenVerzekeraarArbodienst/2019` |
| Versie | 2019.1 |
| Elementen | 167 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`Message`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** |  | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` |  | 1..1 | an..5 | 00701 |
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
| &emsp;&emsp;`IndERDWGA` |  | 0..1 | an1 | J, N |
| &emsp;&emsp;`IndERDZW` |  | 0..1 | an1 | J, N |
| &emsp;&emsp;**`Com`** |  | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`SrtComCd` |  | 1..1 | an2 | 01, 02, 04 |
| &emsp;&emsp;&emsp;`NrCom` |  | 1..1 | an..512 |  |
| &emsp;&emsp;**`Cntprsn`** |  | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`IdWrknmr` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`Persnr` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`Achternaam` |  | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;`Voorl` |  | 0..1 | an..6 |  |
| &emsp;&emsp;&emsp;`Roepnaam` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`GslchtCd` |  | 0..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;`RolCntprsnCd` |  | 0..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;**`Com`** |  | 1..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`SrtComCd` |  | 1..1 | an2 | 01, 02, 04 |
| &emsp;&emsp;&emsp;&emsp;`NrCom` |  | 1..1 | an..512 |  |
| &emsp;&emsp;**`Wrknmr`** |  | 1..* | groep |  |
| &emsp;&emsp;&emsp;`VrwrkCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;`IngdatMut` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Gebdat` |  | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`Overldat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`SignNm` |  | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;`Voorl` |  | 1..1 | an..6 |  |
| &emsp;&emsp;&emsp;`Voorv` |  | 0..1 | an..10 |  |
| &emsp;&emsp;&emsp;`Roepnaam` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`TitVNm` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`TitANm` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`NmvrkrCd` |  | 1..1 | an2 | 01, 02, 03, 04, 99 |
| &emsp;&emsp;&emsp;`GslchtCd` |  | 1..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;`IdWrknmr` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`IdWrknmrOud` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`IdWrknmrArbdnst` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`IdWrknmrVzkr` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;**`Prtnr`** |  | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`VrwrkCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;`SignNm` |  | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;&emsp;`Voorv` |  | 0..1 | an..10 |  |
| &emsp;&emsp;&emsp;**`StrAdrNl`** |  | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`SrtAdrsCd` |  | 1..1 | an2 | 01, 06 |
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
| &emsp;&emsp;&emsp;&emsp;`SrtAdrsCd` |  | 1..1 | an2 | 01, 06 |
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
| &emsp;&emsp;&emsp;**`Com`** |  | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`SrtComCd` |  | 1..1 | an2 | 01, 02, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;`NrCom` |  | 1..1 | an..512 |  |
| &emsp;&emsp;&emsp;**`Dnstvbnd`** |  | 1..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`VrwrkCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;`IngdatMut` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`IdDnstvbnd` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`IdDnstvbndOud` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`DGAJN` |  | 0..1 | an1 | J, N, O |
| &emsp;&emsp;&emsp;&emsp;`RdEndDnstvbndCd` |  | 0..1 | an2 | 01, 02, 03, 05, 06, 07, 08, 09, 10, 99 |
| &emsp;&emsp;&emsp;&emsp;`PersNr` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`PersNrOud` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`CntrnrArbdnst` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`SrtDnstvbndCd` |  | 0..1 | an2 | 19 waarden, o.a. 01, 02, 03, 04, 05 … |
| &emsp;&emsp;&emsp;&emsp;`Fnctcd` |  | 0..1 | an..15 |  |
| &emsp;&emsp;&emsp;&emsp;`NmFnct` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`NmOrgeenh` |  | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`OrgeenhCd` |  | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`OndOrgeenhCd` |  | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`OndOrgeenhCdNm` |  | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`PcStandplts` |  | 0..1 | an..9 |  |
| &emsp;&emsp;&emsp;&emsp;`VrdlngCd` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;`CdBepTd` |  | 0..1 | an1 | B, O |
| &emsp;&emsp;&emsp;&emsp;`CntrctUrnWk` |  | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;&emsp;`DltfctNVS` |  | 0..1 | n..5,2 |  |
| &emsp;&emsp;&emsp;&emsp;`SrtVarWrktdCd` |  | 0..1 | an2 | 01, 02, 03, 04 |
| &emsp;&emsp;&emsp;&emsp;`AantLnwchtdgn` |  | 0..1 | n..3 |  |
| &emsp;&emsp;&emsp;&emsp;`PrcLndrbtng` |  | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;&emsp;**`Arbeidsrelatie`** |  | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`VrwrkCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`IdArbeidsrelatie` |  | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`IdArbeidsrelatieOud` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`PersNr` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`PersNrOud` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Ingdat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`IngdatMut` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Enddat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`AantCtrcturenPWk` |  | 0..1 | n..5,2 |  |
| &emsp;&emsp;&emsp;&emsp;**`Vrzm`** |  | 1..99 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`VrwrkCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`IngdatMutVrzm` |  | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`IngdatMutVrzmOud` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`VrzmgvlId` |  | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`VrzmgvlIdOud` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`VrzmgvlVnrMld` |  | 1..1 | n..3 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`EndVrzmJN` |  | 1..1 | an1 | J, N |
| &emsp;&emsp;&emsp;&emsp;&emsp;`DatVrzmWrkgvr` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`DatEerstVrzmdg` |  | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`DatEerstVrzmdgOud` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`DatHrstld` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`DatHrstldWrkgvr` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`PrcVrzm` |  | 1..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`BijzRdnStartVrzmCd` |  | 0..1 | an2 | 01, 02, 03, 04 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`OorzkVrzmCd` |  | 1..1 | an2 | 11, 99 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`VngntJN` |  | 1..1 | an1 | J, N, O |
| &emsp;&emsp;&emsp;&emsp;&emsp;`RdnEndVrzmCd` |  | 0..1 | an2 | 01, 03, 04, 05, 07, 08, 09, 10, 11, 12, 13, 99 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`RdnEndVrzmBegeleidingCd` |  | 0..1 | an2 | 01, 02, 03, 04, 05, 06, 99 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`WAZOCd` |  | 0..1 | an2 | 01, 02, 03 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`NrUitkBdrver` |  | 0..1 | n..3 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`PrcArbther` |  | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;**`Cntprsn`** |  | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`IdWrknmr` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`Persnr` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`Achternaam` |  | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`Voorl` |  | 0..1 | an..6 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`Roepnaam` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`GslchtCd` |  | 0..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`RolCntprsnCd` |  | 0..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;**`Com`** |  | 1..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`SrtComCd` |  | 1..1 | an2 | 01, 02, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`NrCom` |  | 1..1 | an..512 |  |
| &emsp;&emsp;&emsp;&emsp;**`Cntprsn`** |  | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`IdWrknmr` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Persnr` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Achternaam` |  | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Voorl` |  | 0..1 | an..6 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Roepnaam` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`GslchtCd` |  | 0..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;&emsp;&emsp;`RolCntprsnCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;&emsp;**`Com`** |  | 1..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`SrtComCd` |  | 1..1 | an2 | 01, 02, 04 |
| &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;`NrCom` |  | 1..1 | an..512 |  |
