# Rapportage Arbodiensten - Verzekeraars

Verzuimstandaard Arbodiensten ↔ Verzekeraars, release 2019.

| | |
|---|---|
| Schema | [`xsd/RapportageArbodienst-Verzekeraar.xsd`](../xsd/RapportageArbodienst-Verzekeraar.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/RapportageArbodienstVerzekeraar/2019` |
| Versie | 2019.1 |
| Elementen | 70 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`Message`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** |  | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` |  | 1..1 | an..5 | 00703 |
| &emsp;&emsp;`VnrBrCd` |  | 1..1 | an..5 | 00001 |
| &emsp;&emsp;`AandatBr` |  | 1..1 | datum |  |
| &emsp;&emsp;`AantijdBr` |  | 1..1 | tijd |  |
| &emsp;&emsp;`IdInzndr` |  | 1..1 | an..40 |  |
| &emsp;&emsp;`IdOntvngr` |  | 1..1 | an..40 |  |
| &emsp;&emsp;`Berrefnr` |  | 1..1 | an..512 |  |
| &emsp;&emsp;`TestJN` |  | 1..1 | an1 | J, N, O |
| &emsp;&emsp;`OntvngstbevJN` |  | 1..1 | an1 | J, N, O |
| &emsp;**`VrzkrVolmacht`** |  | 0..1 | groep |  |
| &emsp;&emsp;`HndlsnmOrg` |  | 1..1 | an..100 |  |
| &emsp;&emsp;`IdVrzkrVolmachtCd` |  | 1..1 | an..4 |  |
| &emsp;**`Arbdnst`** |  | 0..1 | groep |  |
| &emsp;&emsp;`HndlsnmOrg` |  | 1..1 | an..100 |  |
| &emsp;&emsp;`ArbdnstCd` |  | 0..1 | an3 |  |
| &emsp;**`Verslagperiode`** |  | 1..999 | groep |  |
| &emsp;&emsp;`Ingdat` |  | 1..1 | datum |  |
| &emsp;&emsp;`Enddat` |  | 1..1 | datum |  |
| &emsp;&emsp;**`Rapportage`** |  | 1..1 | groep |  |
| &emsp;&emsp;&emsp;`AantalKlanten` |  | 1..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalMeldingen` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalVerzuimmeldingen` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalVerzuimdagen` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`Verzuimpercentage` |  | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`Verzuimfrequentie` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalDeelherstelmeldingen` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentageDeelherstelmeldingen` |  | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`AantalHerstelmeldingen` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentageHerstelmeldingen` |  | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`AantalMeldingenRegres` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`GemiddeldeVerzuimduur` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`ZiekteverzuimpercentageKort` |  | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`ZiekteverzuimpercentageMiddellang` |  | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`ZiekteverzuimpercentageLang` |  | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`ZiekteverzuimpercentageExtraLang` |  | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`AantalMeldingenVerzuimKort` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalMeldingenVerzuimMiddellang` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalMeldingenVerzuimLang` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalMeldingenVerzuimExtraLang` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalZiekdagenKort` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalZiekdagenMiddellang` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalZiekdagenLang` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalZiekdagenExtraLang` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalProbleemanalysesOpgesteld` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentageProbleemanalysesOpTijd` |  | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`AantalPlannenVanAanpakOpgesteld` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentagePlannenVanAanpakOpTijd` |  | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`AantalTweeenveertigWeeksmeldingenGedaan` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentageTweeenveertigWeeksmeldingenOpTijd` |  | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`AantalEindejaarsevaluatiesGedaan` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentageEindejaarsevaluatiesOpTijd` |  | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`AantalReintegratieverslagenOpgesteld` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentageReintegratieverslagenOpTijd` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalPoortwachtersancties` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalGeadviseerdeInterventies` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalGeaccordeerdeInterventies` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalInterventiesMetBijdrageVerzekeraar` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`KostenInterventiesVootVerzekeraar` |  | 0..1 | n..9,2 |  |
| &emsp;&emsp;&emsp;`AantalTweedeSpoor` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalPsychischeInterventies` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalFysiekeInterventies` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalMultidisciplinaireInterventies` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalWachtlijstbemiddelingen` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalOverigeInterventies` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`Werkgevertevredenheid` |  | 0..1 | n..3 |  |
| &emsp;&emsp;&emsp;`AantalGemeldeKlachten` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalTerechteKlachten` |  | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentageTerechteKlachten` |  | 0..1 | n..6,2 |  |
