# Rapportage Arbodiensten - Verzekeraars

Verzuimstandaard Arbodiensten ↔ Verzekeraars, release 2022.

| | |
|---|---|
| Schema | [`xsd/RapportageArbodienst-Verzekeraar.xsd`](../xsd/RapportageArbodienst-Verzekeraar.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/RapportageArbodienstVerzekeraar/2022` |
| Versie | 2022.0 |
| Elementen | 71 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`RapportageArbodienstVerzekeraar`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** | Bericht algemeen | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` | an..5 | 1..1 | an..5 | 00703 |
| &emsp;&emsp;`VnrBrCd` | an..5 | 1..1 | an..5 | 00002 |
| &emsp;&emsp;`AandatBr` | an10 | 1..1 | datum |  |
| &emsp;&emsp;`AantijdBr` | an8 | 1..1 | tijd |  |
| &emsp;&emsp;`IdInzndr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;`GebrSwPakket` | an..35 | 1..1 | an..35 |  |
| &emsp;&emsp;`IdOntvngr` | an..40 | 1..1 | an..40 |  |
| &emsp;&emsp;`Berrefnr` | an..512 | 1..1 | an..512 |  |
| &emsp;&emsp;`TestJN` | a1 | 1..1 | an1 | J, N, O |
| &emsp;&emsp;`OntvngstbevJN` | a1 | 1..1 | an1 | J, N, O |
| &emsp;**`VrzkrVolmacht`** | Verzekeraar/volmacht | 0..1 | groep |  |
| &emsp;&emsp;`HndlsnmOrg` | an..100 | 1..1 | an..100 |  |
| &emsp;&emsp;`IdVrzkrVolmachtCd` | an..4 | 1..1 | an..4 |  |
| &emsp;**`Arbdnst`** | Arbodienst | 0..1 | groep |  |
| &emsp;&emsp;`HndlsnmOrg` | an..100 | 1..1 | an..100 |  |
| &emsp;&emsp;`ArbdnstCd` | an3 | 0..1 | an3 |  |
| &emsp;**`Verslagperiode`** | Verslagperiode | 1..999 | groep |  |
| &emsp;&emsp;`Ingdat` | an10 | 1..1 | datum |  |
| &emsp;&emsp;`Enddat` | an10 | 1..1 | datum |  |
| &emsp;&emsp;**`Rapportage`** | Rapportage | 1..1 | groep |  |
| &emsp;&emsp;&emsp;`AantalKlanten` | n..7 | 1..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalMeldingen` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalVerzuimmeldingen` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalVerzuimdagen` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`Verzuimpercentage` | n..6,2 | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`Verzuimfrequentie` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalDeelherstelmeldingen` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentageDeelherstelmeldingen` | n..6,2 | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`AantalHerstelmeldingen` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentageHerstelmeldingen` | n..6,2 | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`AantalMeldingenRegres` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`GemiddeldeVerzuimduur` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`ZiekteverzuimpercentageKort` | n..6,2 | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`ZiekteverzuimpercentageMiddellang` | n..6,2 | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`ZiekteverzuimpercentageLang` | n..6,2 | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`ZiekteverzuimpercentageExtraLang` | n..6,2 | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`AantalMeldingenVerzuimKort` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalMeldingenVerzuimMiddellang` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalMeldingenVerzuimLang` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalMeldingenVerzuimExtraLang` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalZiekdagenKort` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalZiekdagenMiddellang` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalZiekdagenLang` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalZiekdagenExtraLang` | Copyright SIVI | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalProbleemanalysesOpgesteld` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentageProbleemanalysesOpTijd` | n..6,2 | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`AantalPlannenVanAanpakOpgesteld` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentagePlannenVanAanpakOpTijd` | n..6,2 | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`AantalTweeenveertigWeeksmeldingenGedaan` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentageTweeenveertigWeeksmeldingenOpTijd` | n..6,2 | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`AantalEindejaarsevaluatiesGedaan` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentageEindejaarsevaluatiesOpTijd` | n..6,2 | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`AantalReintegratieverslagenOpgesteld` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentageReintegratieverslagenOpTijd` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalPoortwachtersancties` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalGeadviseerdeInterventies` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalGeaccordeerdeInterventies` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalInterventiesMetBijdrageVerzekeraar` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`KostenInterventiesVootVerzekeraar` | n..9,2 | 0..1 | n..9,2 |  |
| &emsp;&emsp;&emsp;`AantalTweedeSpoor` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalPsychischeInterventies` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalFysiekeInterventies` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalMultidisciplinaireInterventies` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalWachtlijstbemiddelingen` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalOverigeInterventies` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`Werkgevertevredenheid` | n..3 | 0..1 | n..3 |  |
| &emsp;&emsp;&emsp;`AantalGemeldeKlachten` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalTerechteKlachten` | n..7 | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentageTerechteKlachten` | Copyright SIVI | 0..1 | n..6,2 |  |
