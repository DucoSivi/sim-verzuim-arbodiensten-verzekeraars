# Uitwisselen Koppelcontractgegevens

Verzuimstandaard Arbodiensten ↔ Verzekeraars, release 2024.

| | |
|---|---|
| Schema | [`xsd/UitwisselenKoppelcontractgegevens.xsd`](../xsd/UitwisselenKoppelcontractgegevens.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/UitwisselenKoppelcontractgegevens/2024` |
| Versie | 2024.0 |
| Elementen | 154 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`UitwisselenKoppelcontractgegevens`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** | Bericht algemeen | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` | Bericht, code | 1..1 | an..5 | 00700 |
| &emsp;&emsp;`VnrBrCd` | Versienummer bericht, code | 1..1 | an..5 | 00004 |
| &emsp;&emsp;`FunctieBrCd` | Functie bericht, code | 1..1 | an2 | 01, 02, 03, 04 |
| &emsp;&emsp;`AandatBr` | Aanmaakdatum bericht | 1..1 | datum |  |
| &emsp;&emsp;`AantijdBr` | Aanmaaktijd bericht | 1..1 | tijd |  |
| &emsp;&emsp;`IdInzndr` | Identificatie inzender | 1..1 | an..40 |  |
| &emsp;&emsp;`GebrSwPakket` | Gebruikt softwarepakket | 1..1 | an..35 |  |
| &emsp;&emsp;`IdOntvngr` | Identificatie ontvanger | 1..1 | an..40 |  |
| &emsp;&emsp;`Berrefnr` | Berichtreferentienummer | 1..1 | an..512 |  |
| &emsp;&emsp;`BerrefnrIngzndnBer` | Berichtreferentienummer ingezonden bericht | 0..1 | an..512 |  |
| &emsp;&emsp;`TestJN` | Test J/N | 1..1 | an1 | J, N |
| &emsp;&emsp;`OntvngstbevJN` | Ontvangstbevestiging gewenst J/N | 1..1 | an1 | J, N |
| &emsp;&emsp;`CntrctGegGewenstJN` | Contractgegevens gewenst J/N | 1..1 | an1 | J, N |
| &emsp;**`VrzkrVolmacht`** | Verzekeraar/volmacht | 1..1 | groep |  |
| &emsp;&emsp;`HndlsnmOrg` | Handelsnaam organisatie | 1..1 | an..100 |  |
| &emsp;&emsp;`IdVrzkrVolmachtCd` | Identificatie verzekeraar/volmacht, code | 1..1 | an..4 |  |
| &emsp;**`Arbdnst`** | Arbodienst | 1..1 | groep |  |
| &emsp;&emsp;`HndlsnmOrg` | Handelsnaam organisatie | 0..1 | an..100 |  |
| &emsp;&emsp;`ArbdnstCd` | Arbodienst, code | 1..1 | an3 |  |
| &emsp;**`Wrkgvr`** | Werkgever | 1..* | groep |  |
| &emsp;&emsp;`VrwrkCd` | Verwerking, code | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;`HndlsnmOrg` | Handelsnaam organisatie | 1..1 | an..100 |  |
| &emsp;&emsp;`InschrijvingsnrKvK` | Inschrijvingsnummer Kamer van Koophandel | 0..1 | n..8 |  |
| &emsp;&emsp;`VestigingsnrHandelsregister` | Vestigingsnummer | 0..1 | n..12 |  |
| &emsp;&emsp;`IdWrkgvrArbdnst` | Identificatie werkgever bij arbodienst | 0..1 | an..40 |  |
| &emsp;&emsp;`AansltnrGeguitwlngArbdnst` | Aansluitnummer gegevensuitwisseling Arbodienst | 0..1 | an..70 |  |
| &emsp;&emsp;`RdnGnGgvnsuitw` | Reden geen gegevensuitwisseling, code | 0..1 | an..2 | 01, 02, 03 |
| &emsp;&emsp;`IDWrkgvrVerzekeraar` | Identificatie werkgever bij verzekeraar | 0..1 | an..40 |  |
| &emsp;&emsp;`IdWrkgvrUWV` | Identificatie werkgever bij UWV | 0..1 | an..40 |  |
| &emsp;&emsp;`Lhnr` | Loonheffingennummer | 0..1 | an..12 |  |
| &emsp;&emsp;`IdVrzkrWGACd` | Identificatie verzekeraar ERD WGA, code | 0..1 | an..4 |  |
| &emsp;&emsp;`IdVrzkrERDZWCd` | Identificatie verzekeraar ERD ZW, code | 0..1 | an..4 |  |
| &emsp;&emsp;`IdVrzkrCollectieveZorgCd` | Identificatie verzekeraar collectieve zorg, code | 0..1 | an..4 |  |
| &emsp;&emsp;`SectorVolgensSBI` | Sector volgens SBI | 0..1 | n..5 |  |
| &emsp;&emsp;**`Personeelssterkte`** | Personeelssterkte | 0..999 | groep |  |
| &emsp;&emsp;&emsp;`PeildatPersoneelssterkte` | Peildatum personeelssterkte | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`VorigePeildatPersoneelssterkte` | Copyright SIVI | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`AantWrknmrs` | Aantal werknemers | 1..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantWrknmrsInDienstSindsVorigePeildat` | Aantal werknemers in dienst sinds vorige peildatum | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantWrknmrsUitDienstSindsVorigePeildat` | Aantal werknemers uit dienst sinds vorige peildatum | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalNulurencntrcten` | Aantal nulurencontracten | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantFTE` | Aantal FTE | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantVrouwelijkeWrknmrs` | Aantal vrouwelijke werknemers | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;`AantVrouwelijkeFTE` | Aantal vrouwelijke FTE | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;`AantMannelijkeWrknmrs` | Aantal mannelijke werknemers | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;`AantMannelijkeFTE` | Aantal mannelijke FTE | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;`AantUrenFTE` | Aantal uren FTE | 0..1 | n..3 |  |
| &emsp;&emsp;**`StrAdrNl`** | Straatadres nederland | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`SrtAdrsCd` | Soort adres, code | 0..1 | an2 | 01, 02, 03, 05 |
| &emsp;&emsp;&emsp;`Ingdat` | Ingangsdatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | Einddatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Pc` | Postcode | 1..1 | an6 |  |
| &emsp;&emsp;&emsp;`Wnpl` | Woonplaatsnaam | 0..1 | an..24 |  |
| &emsp;&emsp;&emsp;`StraatLang` | Straatnaam_ | 0..1 | an..80 |  |
| &emsp;&emsp;&emsp;`Huisnr` | Huisnummer | 1..1 | n..5 |  |
| &emsp;&emsp;&emsp;`HuisToev` | Huisnummertoevoeging | 0..1 | an..4 |  |
| &emsp;&emsp;**`StrAdrBl`** | Straatadres buitenland | 0..* | groep |  |
| &emsp;&emsp;&emsp;`SrtAdrsCd` | Soort adres, code | 0..1 | an2 | 01, 02, 03, 05 |
| &emsp;&emsp;&emsp;`Ingdat` | Ingangsdatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | Einddatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`LocomsBtl` | Locatieomschrijving buitenland | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`PcBtl` | Postcode buitenland | 0..1 | an..9 |  |
| &emsp;&emsp;&emsp;`WnplBtl` | Woonplaatsnaam buitenland | 1..1 | an..24 |  |
| &emsp;&emsp;&emsp;`RegBtl` | Regionaam buitenland | 0..1 | an..24 |  |
| &emsp;&emsp;&emsp;`LandCd` | Land, code | 1..1 | an2 |  |
| &emsp;&emsp;&emsp;`Landnm` | Landnaam | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`StraatLang` | Straatnaam_ | 0..1 | an..80 |  |
| &emsp;&emsp;&emsp;`HuisnrBtl` | Huisnummer buitenland | 1..1 | an..9 |  |
| &emsp;&emsp;&emsp;`HuisnrToevBtl` | Huisnummer toevoeging buitenland | 0..1 | an..70 |  |
| &emsp;&emsp;**`AdministratieveEenheid`** | Administratieve eenheid | 0..1 | groep |  |
| &emsp;&emsp;&emsp;`NmIp` | Naam inhoudingsplichtige | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;`LhNr` | Loonheffingennummer | 0..1 | an..12 |  |
| &emsp;&emsp;**`OrgEenh`** | Organisatie eenheid | 0..999 | groep |  |
| &emsp;&emsp;&emsp;`VrwrkCd` | Verwerking, code | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;`IngdatMut` | Ingangsdatum mutatie | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`NmOrgeenh` | Naam organisatie-eenheid | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;`OrgeenhCd` | Organisatie-eenheid, code | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;`OndOrgeenhCd` | Onderdeel van organisatieeenheid, code | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;**`Personeelssterkte`** | Personeelssterkte | 0..* | groep |  |
| &emsp;&emsp;&emsp;&emsp;`PeildatPersoneelssterkte` | Peildatum personeelssterkte | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`VorigePeildatPersoneelssterkte` | Copyright SIVI | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`AantWrknmrs` | Aantal werknemers | 1..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantWrknmrsInDienstSindsVorigePeildat` | Aantal werknemers in dienst sinds vorige peildatum | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantWrknmrsUitDienstSindsVorigePeildat` | Aantal werknemers uit dienst sinds vorige peildatum | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantalNulurencntrcten` | Aantal nulurencontracten | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantFTE` | Aantal FTE | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;&emsp;`AantVrouwelijkeWrknmrs` | Aantal vrouwelijke werknemers | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantVrouwelijkeFTE` | Aantal vrouwelijke FTE | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantMannelijkeWrknmrs` | Aantal mannelijke werknemers | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantMannelijkeFTE` | Aantal mannelijke FTE | 0..1 | n..5 |  |
| &emsp;&emsp;&emsp;&emsp;`AantUrenFTE` | Aantal uren FTE | 0..1 | n..3 |  |
| &emsp;&emsp;**`ArboCntrct`** | Arbocontract | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`VrwrkCd` | Verwerking, code | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;`Cntrnr` | Contractnummer | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;`Ingdat` | Ingangsdatum | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`IngdatMut` | Ingangsdatum mutatie | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | Einddatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`StatusCntrctCd` | Status contract, code | 1..1 | an2 | 01, 02 |
| &emsp;&emsp;&emsp;`TypArbContCod` | Type arbocontract, code | 1..1 | an..2 | 01, 02, 03 |
| &emsp;&emsp;&emsp;**`Intermediair`** | Intermediair | 0..1 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`HndlsnmOrg` | Handelsnaam organisatie | 1..1 | an..100 |  |
| &emsp;&emsp;&emsp;&emsp;**`Com`** | Communicatie | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;&emsp;`SrtComCd` | Soort communicatie, code | 1..1 | an2 | 06, 08, 10 |
| &emsp;&emsp;&emsp;&emsp;&emsp;`NrCom` | Nummer/adres communicatie | 1..1 | an..512 |  |
| &emsp;&emsp;&emsp;**`Dnstvrlnng`** | Dienstverlening | 0..9 | groep |  |
| &emsp;&emsp;&emsp;&emsp;`VrwrkCd` | Verwerking, code | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;&emsp;`DnstvrlnngId` | Identificatie dienstverlening | 1..1 | an..40 |  |
| &emsp;&emsp;&emsp;&emsp;`TypeArbopakketCd` | Type arbopakket, code | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`TypeArbopakketOms` | Type arbopakket, omschrijving | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;&emsp;`RdnEindDnstvrl` | Reden einde dienstverlening, code | 0..1 | an..2 | 01, 02, 03 |
| &emsp;&emsp;&emsp;&emsp;`Ingdat` | Ingangsdatum | 1..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`IngdatMut` | Ingangsdatum mutatie | 0..1 | datum |  |
| &emsp;&emsp;&emsp;&emsp;`Enddat` | Einddatum | 0..1 | datum |  |
| &emsp;&emsp;**`Verzekering`** | Verzekering/dekking | 0..99 | groep |  |
| &emsp;&emsp;&emsp;`VrwrkCd` | Verwerking, code | 1..1 | an2 | 01, 02, 03, 04, 05 |
| &emsp;&emsp;&emsp;`Cntrnr` | Contractnummer | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`CntrnrPakket` | Contractnummer pakket | 0..1 | an..40 |  |
| &emsp;&emsp;&emsp;`Ingdat` | Ingangsdatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`IngdatMut` | Ingangsdatum mutatie | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | Einddatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`CntrctPerCd` | Contract periode | 0..1 | an..2 | 01, 02, 03, 04, 05, 06 |
| &emsp;&emsp;&emsp;`StatusCntrctCd` | Status contract, code | 1..1 | an2 | 01, 02 |
| &emsp;&emsp;&emsp;`RdnBeeindCntrct` | Reden beëindiging contract, code | 0..1 | an2 | 01, 02, 03, 04, 05, 06, 07, 08, 99 |
| &emsp;&emsp;&emsp;`SrtVerzekeringCd` | Soort verzekering, gecodeerd | 1..1 | an2 | 01, 02, 03, 04, 05, 06, 07, 08, 09, 10 |
| &emsp;&emsp;&emsp;`WachttijdInDgn` | Wachttijd in werkdagen | 0..1 | n..3 |  |
| &emsp;&emsp;&emsp;`LoonsrtCd` | Loonsoort | 0..1 | an..2 | 01, 02, 03, 04 |
| &emsp;&emsp;&emsp;`MaxJrLoonVrzkrd` | Maximum verzekerd jaarloon | 0..1 | n..9,2 |  |
| &emsp;&emsp;&emsp;`PrcDkkngJr1` | Dekkingspercentage jaar 1 | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`PrcDkkngJr2` | Dekkingspercentage jaar 2 | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`PercWrkgvrslasten` | Percentage werkgeverslasten | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`Productkenmerk` | Productkenmerk | 0..1 | an..70 |  |
| &emsp;&emsp;&emsp;`InloopJN` | Inloop J/N | 1..1 | an1 | J, N |
| &emsp;&emsp;&emsp;`UitloopJN` | Uitloop J/N | 1..1 | an1 | J, N |
| &emsp;&emsp;**`MchtVrzm`** | Machtigingen uitwisseling verzuim | 0..1 | groep |  |
| &emsp;&emsp;&emsp;`VrwrkCd` | Verwerking, code | 1..1 | an2 | 01, 02, 04 |
| &emsp;&emsp;&emsp;`Ingdat` | Ingangsdatum | 1..1 | datum |  |
| &emsp;&emsp;&emsp;`Enddat` | Einddatum | 0..1 | datum |  |
| &emsp;&emsp;&emsp;`KpplCd` | Koppelcode | 1..1 | an..70 |  |
| &emsp;&emsp;&emsp;`RdnEndMCd` | Reden einde machtiging, code | 0..1 | an2 | 01, 02, 03, 04 |
| &emsp;&emsp;**`Com`** | Communicatie | 0..9 | groep |  |
| &emsp;&emsp;&emsp;`SrtComCd` | Soort communicatie, code | 1..1 | an2 | 01, 02, 04 |
| &emsp;&emsp;&emsp;`NrCom` | Nummer/adres communicatie | 1..1 | an..512 |  |
| &emsp;&emsp;**`Cntprsn`** | Contactpersoon | 0..* | groep |  |
| &emsp;&emsp;&emsp;`Persnr` | Copyright SIVI | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`Achternaam` | Achternaam/Achternamen | 1..1 | an..200 |  |
| &emsp;&emsp;&emsp;`Voorl` | Voorletters | 1..1 | an..6 |  |
| &emsp;&emsp;&emsp;`Roepnaam` | Roepnaam | 0..1 | an..35 |  |
| &emsp;&emsp;&emsp;`GslchtCd` | Geslachtsaanduiding, code | 1..1 | an1 | M, O, V |
| &emsp;&emsp;&emsp;`RolCntprsnCd` | Rol contactpersoon, code | 0..1 | an2 | 02, 03, 05 |
| &emsp;&emsp;&emsp;**`Com`** | Communicatie | 0..* | groep |  |
| &emsp;&emsp;&emsp;&emsp;`SrtComCd` | Soort communicatie, code | 1..1 | an2 | 06, 08, 10 |
| &emsp;&emsp;&emsp;&emsp;`NrCom` | Nummer/adres communicatie | 1..1 | an..512 |  |
