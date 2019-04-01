# Uitwisselen Koppelcontractgegevens

Verzuimstandaard Arbodiensten ↔ Verzekeraars, release 2019.

| | |
|---|---|
| Schema | [`xsd/UitwisselenKoppelcontractgegevens.xsd`](../xsd/UitwisselenKoppelcontractgegevens.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/UitwisselenKoppelcontractgegevens/2019` |
| Versie | 2019.1 |
| Elementen | 179 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`Message`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** |  | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` |  | 1..1 | an..5 | 00700 |
| &emsp;&emsp;`VnrBrCd` |  | 1..1 | an..5 | 00001 |
| &emsp;&emsp;`FunctieBrCd` |  | 1..1 | an2 | 01, 02, 03, 04 |
| &emsp;&emsp;`AandatBr` |  | 1..1 | datum |  |
| &emsp;&emsp;`AantijdBr` |  | 1..1 | tijd |  |
| &emsp;&emsp;`IdInzndr` |  | 1..1 | an..40 |  |
| &emsp;&emsp;`IdOntvngr` |  | 1..1 | an..40 |  |
| &emsp;&emsp;`Berrefnr` |  | 1..1 | an..512 |  |
| &emsp;&emsp;`BerrefnrIngzndnBer` |  | 0..1 | an..512 |  |
| &emsp;&emsp;`TestJN` |  | 1..1 | an1 | J, N |
| &emsp;&emsp;`OntvngstbevJN` |  | 1..1 | an1 | J, N |
| &emsp;&emsp;`CntrctGegGewenstJN` |  | 1..1 | an1 | J, N |
| &emsp;**`VrzkrVolmacht`** |  | 1..1 | groep |  |
| &emsp;&emsp;`HndlsnmOrg` |  | 1..1 | an..100 |  |
| &emsp;&emsp;`IdVrzkrVolmachtCd` |  | 1..1 | an..4 |  |
| &emsp;**`Arbdnst`** |  | 1..1 | groep |  |
| &emsp;&emsp;`HndlsnmOrg` |  | 0..1 | an..100 |  |
| &emsp;&emsp;`ArbdnstCd` |  | 1..1 | an3 |  |
| &emsp;**`Wrkgvr`** |  | 1..* | groep |  |
| &emsp;&emsp;`VrwrkCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;`HndlsnmOrg` |  | 1..1 | an..100 |  |
| &emsp;&emsp;`InschrijvingsnrKvK` |  | 0..1 | n..8 |  |
| &emsp;&emsp;`VestigingsnrHandelsregister` |  | 0..1 | n..12 |  |
| &emsp;&emsp;`IdWrkgvrArbdnst` |  | 0..1 | an..40 |  |
| &emsp;&emsp;`AansltnrGeguitwlngArbdnst` |  | 0..1 | an..70 |  |
| &emsp;&emsp;`IDWrkgvrVerzekeraar` |  | 0..1 | an..40 |  |
| &emsp;&emsp;`IdWrkgvrUWV` |  | 0..1 | an..40 |  |
| &emsp;&emsp;`Lhnr` |  | 0..1 | an..12 |  |
| &emsp;&emsp;`OrgeenhCd` |  | 1..1 | an..70 |  |
| &emsp;&emsp;`IdVrzkrWGACd` |  | 0..1 | an..4 |  |
| &emsp;&emsp;`IdVrzkrERDZWCd` |  | 0..1 | an..4 |  |
| &emsp;&emsp;`IdVrzkrCollectieveZorgCd` |  | 0..1 | an..4 |  |
| &emsp;&emsp;`SectorVolgensSBI` |  | 0..1 | n..5 |  |
| &emsp;&emsp;**`Personeelssterkte`** |  | 0..999 | groep |  |
| &emsp;&emsp;&emsp;`VrwrkCd` |  | 1..1 | an2 |  |
| &emsp;&emsp;&emsp;`PeildatPersoneelssterkte` |  | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`VorigePeildatPersoneelssterkte` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`AantWrknmrs` |  | 1..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantWrknmrsInDienstSindsVorigePeildat` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantWrknmrsUitDienstSindsVorigePeildat` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalNulurencntrcten` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantFTE` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantVrouwelijkeWrknmrs` |  | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;`AantVrouwelijkeFTE` |  | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;`AantMannelijkeWrknmrs` |  | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;`AantMannelijkeFTE` |  | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;`AantUrenFTE` |  | 0..1 | n..3 |  |
| &emsp;&emsp;**`StrAdrNl`** |  | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`Ingdat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Pc` |  | 1..1 | an6 |  |
| &emsp;&emsp;&emsp;`Wnpl` |  | 0..1 | an..24 |  |
| &emsp;&emsp;&emsp;`StraatLang` |  | 0..1 | an..80 |  |
| &emsp;&emsp;&emsp;`Huisnr` |  | 1..1 | n..5 |  |
| &emsp;&emsp;&emsp;`HuisToev` |  | 0..1 | an..4 |  |
| &emsp;&emsp;**`PbadrsNl`** |  | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`Ingdat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Pc` |  | 1..1 | an6 |  |
| &emsp;&emsp;&emsp;`Wnpl` |  | 0..1 | an..24 |  |
| &emsp;&emsp;&emsp;`Pbnr` |  | 1..1 | n..5 |  |
| &emsp;&emsp;**`StrAdrBl`** |  | 0..* | groep |  |
| &emsp;&emsp;&emsp;`Ingdat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`LocomsBtl` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`PcBtl` |  | 0..1 | an..9 |  |
| &emsp;&emsp;&emsp;`WnplBtl` |  | 1..1 | an..24 |  |
| &emsp;&emsp;&emsp;`RegBtl` |  | 0..1 | an..24 |  |
| &emsp;&emsp;&emsp;`LandCd` |  | 1..1 | an2 |  |
| &emsp;&emsp;&emsp;`Landnm` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`StraatLang` |  | 0..1 | an..80 |  |
| &emsp;&emsp;&emsp;`HuisnrBtl` |  | 1..1 | an..9 |  |
| &emsp;&emsp;&emsp;`HuisnrToevBtl` |  | 0..1 | an..70 |  |
| &emsp;&emsp;**`PostbusadresBuitenland`** |  | 0..* | groep |  |
| &emsp;&emsp;&emsp;`Ingdat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`LocomsBtl` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`PcBtl` |  | 0..1 | an..9 |  |
| &emsp;&emsp;&emsp;`WnplBtl` |  | 1..1 | an..24 |  |
| &emsp;&emsp;&emsp;`RegBtl` |  | 0..1 | an..24 |  |
| &emsp;&emsp;&emsp;`LandCd` |  | 1..1 | an2 |  |
| &emsp;&emsp;&emsp;`Landnm` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`PostbusnummerBuitenland` |  | 1..1 | an..7 |  |
| &emsp;&emsp;**`AdministratieveEenheid`** |  | 0..1 | groep |  |
| &emsp;&emsp;&emsp;`NmIp` |  | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;`LhNr` |  | 0..1 | an..12 |  |
| &emsp;&emsp;**`OrgEenh`** |  | 0..999 | groep |  |
| &emsp;&emsp;&emsp;`VrwrkCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;`IngdatMut` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`NmOrgeenh` |  | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;`OrgeenhCd` |  | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;`OndOrgeenhCd` |  | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;**`Personeelssterkte`** |  | 0..* | groep |  |
| &emsp;&emsp;&emsp;&emsp;`VrwrkCd` |  | 1..1 | an2 |  |
| &emsp;&emsp;&emsp;&emsp;`PeildatPersoneelssterkte` |  | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`VorigePeildatPersoneelssterkte` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`AantWrknmrs` |  | 1..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantWrknmrsInDienstSindsVorigePeildat` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantWrknmrsUitDienstSindsVorigePeildat` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantalNulurencntrcten` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantFTE` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantVrouwelijkeWrknmrs` |  | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantVrouwelijkeFTE` |  | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantMannelijkeWrknmrs` |  | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantMannelijkeFTE` |  | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantUrenFTE` |  | 0..1 | n..3 |  |
| &emsp;&emsp;**`ArboCntrct`** |  | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`VrwrkCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;`Cntrnr` |  | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;`Ingdat` |  | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`IngdatMut` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`StatusCntrctCd` |  | 1..1 | an2 | 01, 02 |
| &emsp;&emsp;&emsp;**`Intermediair`** |  | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`HndlsnmOrg` |  | 1..1 | an..100 |  |
| &emsp;&emsp;&emsp;&emsp;**`StrAdrNl`** |  | 0..* | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Pc` |  | 1..1 | an6 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Wnpl` |  | 1..1 | an..24 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`StraatLang` |  | 1..1 | an..80 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Huisnr` |  | 1..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`HuisToev` |  | 0..1 | an..4 |  |
| &emsp;&emsp;&emsp;&emsp;**`Com`** |  | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`SrtComCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05, 98, 99 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`NrCom` |  | 1..1 | an..512 |  |
| &emsp;&emsp;&emsp;**`Dnstvrlnng`** |  | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`VrwrkCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;`DnstvrlnngId` |  | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`TypeArbopakketCd` |  | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`TypeArbopakketOms` |  | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` |  | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`IngdatMut` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` |  | 0..1 | datum |  |
| &emsp;&emsp;**`Verzekering`** |  | 0..99 | groep |  |
| &emsp;&emsp;&emsp;`VrwrkCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;`Cntrnr` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`CntrnrPakket` |  | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`Ingdat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`IngdatMut` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`CntrctPerCd` |  | 0..1 | an..2 | 01, 02, 03, 04, 05, 06 |
| &emsp;&emsp;&emsp;`StatusCntrctCd` |  | 1..1 | an2 | 01, 02 |
| &emsp;&emsp;&emsp;`RdnBeeindCntrct` |  | 0..1 | an2 | 01, 02, 03, 04, 05, 06, 99 |
| &emsp;&emsp;&emsp;`SrtVerzekeringCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05, 06, 07, 08, 09, 10 |
| &emsp;&emsp;&emsp;`WachttijdInDgn` |  | 0..1 | n..3 |  |
| &emsp;&emsp;&emsp;`LoonsrtCd` |  | 0..1 | an..2 | 01, 02, 03, 04 |
| &emsp;&emsp;&emsp;`MaxJrLoonVrzkrd` |  | 0..1 | n..9,2 |  |
| &emsp;&emsp;&emsp;`DekkingspercentageJaar1` |  | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`PrcDkkngJr2` |  | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`PercWrkgvrslasten` |  | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`Productkenmerk` |  | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;`InloopJN` |  | 1..1 | an1 | J, N |
| &emsp;&emsp;&emsp;`UitloopJN` |  | 1..1 | an1 | J, N |
| &emsp;&emsp;&emsp;**`AfsprakenUitwisselingVerzuimdata`** |  | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`VrwrkCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` |  | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`UitwisselingVerzuimmeldingenCd` |  | 1..1 | an2 | 01, 02, 99 |
| &emsp;&emsp;&emsp;&emsp;`FrequentieCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;**`AfsprakenUitwisselingVerzuimdata`** |  | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`VrwrkCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;`Ingdat` |  | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` |  | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`UitwisselingVerzuimmeldingenCd` |  | 1..1 | an2 | 01, 02, 99 |
| &emsp;&emsp;&emsp;`FrequentieCd` |  | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;**`Com`** |  | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`SrtComCd` |  | 1..1 | an2 | 01, 02, 04 |
| &emsp;&emsp;&emsp;`NrCom` |  | 1..1 | an..512 |  |
| &emsp;&emsp;**`Cntprsn`** |  | 0..* | groep |  |
| &emsp;&emsp;&emsp;`Persnr` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`Achternaam` |  | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;`Voorl` |  | 1..1 | an..6 |  |
| &emsp;&emsp;&emsp;`Roepnaam` |  | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`GslchtCd` |  | 1..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;`RolCntprsnCd` |  | 0..1 | an2 | 02, 03, 05 |
| &emsp;&emsp;&emsp;**`Com`** |  | 0..* | groep |  |
| &emsp;&emsp;&emsp;&emsp;`SrtComCd` |  | 1..1 | an2 | 01, 02, 04 |
| &emsp;&emsp;&emsp;&emsp;`NrCom` |  | 1..1 | an..512 |  |
