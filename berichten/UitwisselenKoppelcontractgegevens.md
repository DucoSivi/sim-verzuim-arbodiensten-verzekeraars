# Uitwisselen Koppelcontractgegevens

Verzuimstandaard Arbodiensten ↔ Verzekeraars, release 2021.

| | |
|---|---|
| Schema | [`xsd/UitwisselenKoppelcontractgegevens.xsd`](../xsd/UitwisselenKoppelcontractgegevens.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/UitwisselenKoppelcontractgegevens/2021` |
| Versie | 2021.0 |
| Elementen | 178 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`UitwisselenKoppelcontractgegevens`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** | Bericht algemeen | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` | an..5 | 1..1 | an..5 | 00700 |
| &emsp;&emsp;`VnrBrCd` | an..5 | 1..1 | an..5 | 00002 |
| &emsp;&emsp;`FunctieBrCd` | an2 | 1..1 | an2 | 01, 02, 03, 04 |
| &emsp;&emsp;`AandatBr` | an10 | 1..1 | datum |  |
| &emsp;&emsp;`AantijdBr` | an8 | 1..1 | tijd |  |
| &emsp;&emsp;`IdInzndr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;`GebrSwPakket` | an..35 | 1..1 | an..35 |  |
| &emsp;&emsp;`IdOntvngr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;`Berrefnr` | an..512 | 1..1 | an..512 |  |
| &emsp;&emsp;`BerrefnrIngzndnBer` | an..512 | 0..1 | an..512 |  |
| &emsp;&emsp;`TestJN` | a1 | 1..1 | an1 | J, N |
| &emsp;&emsp;`OntvngstbevJN` | a1 | 1..1 | an1 | J, N |
| &emsp;&emsp;`CntrctGegGewenstJN` | a1 | 1..1 | an1 | J, N |
| &emsp;**`VrzkrVolmacht`** | Verzekeraar/volmacht | 1..1 | groep |  |
| &emsp;&emsp;`HndlsnmOrg` | an..100 | 1..1 | an..100 |  |
| &emsp;&emsp;`IdVrzkrVolmachtCd` | an..4 | 1..1 | an..4 |  |
| &emsp;**`Arbdnst`** | Arbodienst | 1..1 | groep |  |
| &emsp;&emsp;`HndlsnmOrg` | an..100 | 0..1 | an..100 |  |
| &emsp;&emsp;`ArbdnstCd` | an3 | 1..1 | an3 |  |
| &emsp;**`Wrkgvr`** | Werkgever | 1..* | groep |  |
| &emsp;&emsp;`VrwrkCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;`HndlsnmOrg` | an..100 | 1..1 | an..100 |  |
| &emsp;&emsp;`InschrijvingsnrKvK` | n..8 | 0..1 | n..8 |  |
| &emsp;&emsp;`VestigingsnrHandelsregister` | n..12 | 0..1 | n..12 |  |
| &emsp;&emsp;`IdWrkgvrArbdnst` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;`AansltnrGeguitwlngArbdnst` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;`IDWrkgvrVerzekeraar` | Copyright SIVI | 0..1 | an..40 |  |
| &emsp;&emsp;`IdWrkgvrUWV` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;`Lhnr` | an..12 | 0..1 | an..12 |  |
| &emsp;&emsp;`OrgeenhCd` | an..70 | 1..1 | an..70 |  |
| &emsp;&emsp;`IdVrzkrWGACd` | an..4 | 0..1 | an..4 |  |
| &emsp;&emsp;`IdVrzkrERDZWCd` | an..4 | 0..1 | an..4 |  |
| &emsp;&emsp;`IdVrzkrCollectieveZorgCd` | an..4 | 0..1 | an..4 |  |
| &emsp;&emsp;`SectorVolgensSBI` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;**`Personeelssterkte`** | Personeelssterkte | 0..999 | groep |  |
| &emsp;&emsp;&emsp;`PeildatPersoneelssterkte` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`VorigePeildatPersoneelssterkte` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`AantWrknmrs` | n..7 | 1..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantWrknmrsInDienstSindsVorigePeildat` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantWrknmrsUitDienstSindsVorigePeildat` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalNulurencntrcten` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantFTE` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantVrouwelijkeWrknmrs` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;`AantVrouwelijkeFTE` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;`AantMannelijkeWrknmrs` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;`AantMannelijkeFTE` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;`AantUrenFTE` | n..3 | 0..1 | n..3 |  |
| &emsp;&emsp;**`StrAdrNl`** | Straatadres nederland | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`Ingdat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Pc` | an6 | 1..1 | an6 |  |
| &emsp;&emsp;&emsp;`Wnpl` | an..24 | 0..1 | an..24 |  |
| &emsp;&emsp;&emsp;`StraatLang` | an..80 | 0..1 | an..80 |  |
| &emsp;&emsp;&emsp;`Huisnr` | n..5 | 1..1 | n..5 |  |
| &emsp;&emsp;&emsp;`HuisToev` | an..4 | 0..1 | an..4 |  |
| &emsp;&emsp;**`PbadrsNl`** | Postbusadres nederland | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`Ingdat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Pc` | an6 | 1..1 | an6 |  |
| &emsp;&emsp;&emsp;`Wnpl` | an..24 | 0..1 | an..24 |  |
| &emsp;&emsp;&emsp;`Pbnr` | n..5 | 1..1 | n..5 |  |
| &emsp;&emsp;**`StrAdrBl`** | Straatadres buitenland | 0..* | groep |  |
| &emsp;&emsp;&emsp;`Ingdat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`LocomsBtl` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`PcBtl` | an..9 | 0..1 | an..9 |  |
| &emsp;&emsp;&emsp;`WnplBtl` | an..24 | 1..1 | an..24 |  |
| &emsp;&emsp;&emsp;`RegBtl` | an..24 | 0..1 | an..24 |  |
| &emsp;&emsp;&emsp;`LandCd` | a2 | 1..1 | an2 |  |
| &emsp;&emsp;&emsp;`Landnm` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`StraatLang` | an..80 | 0..1 | an..80 |  |
| &emsp;&emsp;&emsp;`HuisnrBtl` | an..9 | 1..1 | an..9 |  |
| &emsp;&emsp;&emsp;`HuisnrToevBtl` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;**`PostbusadresBuitenland`** |  | 0..* | groep |  |
| &emsp;&emsp;&emsp;`Ingdat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`LocomsBtl` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`PcBtl` | an..9 | 0..1 | an..9 |  |
| &emsp;&emsp;&emsp;`WnplBtl` | an..24 | 1..1 | an..24 |  |
| &emsp;&emsp;&emsp;`RegBtl` | an..24 | 0..1 | an..24 |  |
| &emsp;&emsp;&emsp;`LandCd` | a2 | 1..1 | an2 |  |
| &emsp;&emsp;&emsp;`Landnm` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`PostbusnummerBuitenland` |  | 1..1 | an..7 |  |
| &emsp;&emsp;**`AdministratieveEenheid`** | Administratieve eenheid | 0..1 | groep |  |
| &emsp;&emsp;&emsp;`NmIp` | an..200 | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;`LhNr` | an..12 | 0..1 | an..12 |  |
| &emsp;&emsp;**`OrgEenh`** | Organisatie eenheid | 0..999 | groep |  |
| &emsp;&emsp;&emsp;`VrwrkCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;`IngdatMut` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`NmOrgeenh` | an..70 | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;`OrgeenhCd` | an..70 | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;`OndOrgeenhCd` | an..70 | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;**`Personeelssterkte`** | Personeelssterkte | 0..* | groep |  |
| &emsp;&emsp;&emsp;&emsp;`PeildatPersoneelssterkte` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`VorigePeildatPersoneelssterkte` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`AantWrknmrs` | n..7 | 1..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantWrknmrsInDienstSindsVorigePeildat` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantWrknmrsUitDienstSindsVorigePeildat` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantalNulurencntrcten` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantFTE` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantVrouwelijkeWrknmrs` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantVrouwelijkeFTE` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantMannelijkeWrknmrs` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantMannelijkeFTE` | n..5 | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantUrenFTE` | n..3 | 0..1 | n..3 |  |
| &emsp;&emsp;**`ArboCntrct`** | Arbocontract | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`VrwrkCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;`Cntrnr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;`Ingdat` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`IngdatMut` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`StatusCntrctCd` | an2 | 1..1 | an2 | 01, 02 |
| &emsp;&emsp;&emsp;**`Intermediair`** | Intermediair | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`HndlsnmOrg` | an..100 | 1..1 | an..100 |  |
| &emsp;&emsp;&emsp;&emsp;**`StrAdrNl`** | Straatadres nederland | 0..* | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Pc` | an6 | 1..1 | an6 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Wnpl` | an..24 | 1..1 | an..24 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`StraatLang` | an..80 | 1..1 | an..80 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`Huisnr` | n..5 | 1..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`HuisToev` | an..4 | 0..1 | an..4 |  |
| &emsp;&emsp;&emsp;&emsp;**`Com`** | Communicatie | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`SrtComCd` | an2 | 1..1 | an2 | 06, 08, 10 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`NrCom` | an..512 | 1..1 | an..512 |  |
| &emsp;&emsp;&emsp;**`Dnstvrlnng`** | Dienstverlening | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`VrwrkCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;`DnstvrlnngId` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`TypeArbopakketCd` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`TypeArbopakketOms` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`IngdatMut` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;**`Verzekering`** | Verzekering/dekking | 0..99 | groep |  |
| &emsp;&emsp;&emsp;`VrwrkCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;`Cntrnr` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`CntrnrPakket` | an..40 | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`Ingdat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`IngdatMut` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`CntrctPerCd` | an..2 | 0..1 | an..2 | 01, 02, 03, 04, 05, 06 |
| &emsp;&emsp;&emsp;`StatusCntrctCd` | an2 | 1..1 | an2 | 01, 02 |
| &emsp;&emsp;&emsp;`RdnBeeindCntrct` | an2 | 0..1 | an2 | 01, 02, 03, 04, 05, 06, 99 |
| &emsp;&emsp;&emsp;`SrtVerzekeringCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05, 06, 07, 08, 09, 10 |
| &emsp;&emsp;&emsp;`WachttijdInDgn` | n..3 | 0..1 | n..3 |  |
| &emsp;&emsp;&emsp;`LoonsrtCd` | an..2 | 0..1 | an..2 | 01, 02, 03, 04 |
| &emsp;&emsp;&emsp;`MaxJrLoonVrzkrd` | n..9,2 | 0..1 | n..9,2 |  |
| &emsp;&emsp;&emsp;`DekkingspercentageJaar1` |  | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`PrcDkkngJr2` | n..6,2 | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`PercWrkgvrslasten` | n..6,2 | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`Productkenmerk` | an..70 | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;`InloopJN` | a1 | 1..1 | an1 | J, N |
| &emsp;&emsp;&emsp;`UitloopJN` | a1 | 1..1 | an1 | J, N |
| &emsp;&emsp;&emsp;**`AfsprakenUitwisselingVerzuimdata`** | Afspraken uitwisseling verzuimdata | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`VrwrkCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`UitwisselingVerzuimmeldingenCd` | an2 | 1..1 | an2 | 01, 02, 99 |
| &emsp;&emsp;&emsp;&emsp;`FrequentieCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;**`AfsprakenUitwisselingVerzuimdata`** | Afspraken uitwisseling verzuimdata | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`VrwrkCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;`Ingdat` | an10 | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | an10 | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`UitwisselingVerzuimmeldingenCd` | an2 | 1..1 | an2 | 01, 02, 99 |
| &emsp;&emsp;&emsp;`FrequentieCd` | an2 | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;**`Com`** | Communicatie | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`SrtComCd` | an2 | 1..1 | an2 | 01, 02, 04 |
| &emsp;&emsp;&emsp;`NrCom` | an..512 | 1..1 | an..512 |  |
| &emsp;&emsp;**`Cntprsn`** | Contactpersoon | 0..* | groep |  |
| &emsp;&emsp;&emsp;`Persnr` | an..35 | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`Achternaam` | an..200 | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;`Voorl` | a..6 | 1..1 | an..6 |  |
| &emsp;&emsp;&emsp;`Roepnaam` | Copyright SIVI | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`GslchtCd` | an1 | 1..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;`RolCntprsnCd` | an2 | 0..1 | an2 | 02, 03, 05 |
| &emsp;&emsp;&emsp;**`Com`** | Communicatie | 0..* | groep |  |
| &emsp;&emsp;&emsp;&emsp;`SrtComCd` | an2 | 1..1 | an2 | 06, 08, 10 |
| &emsp;&emsp;&emsp;&emsp;`NrCom` | an..512 | 1..1 | an..512 |  |
