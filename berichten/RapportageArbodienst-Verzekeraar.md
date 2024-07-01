# Rapportage Arbodiensten - Verzekeraars

Verzuimstandaard Arbodiensten ↔ Verzekeraars, release 2024.

| | |
|---|---|
| Schema | [`xsd/RapportageArbodienst-Verzekeraar.xsd`](../xsd/RapportageArbodienst-Verzekeraar.xsd) |
| Namespace | `http://www.sivi.org/Verzuimmanagement/RapportageArbodienstVerzekeraar/2024` |
| Versie | 2024.0 |
| Elementen | 71 |

Deze pagina is afgeleid van de XSD. De namen komen uit de functionele hiërarchie; de volledige toelichting per element staat in de PDF bij de release.

## Berichtstructuur

| XML-tag | Naam | Voorkomen | Formaat | Toegestane waarden |
|---|---|---|---|---|
| **`RapportageArbodienstVerzekeraar`** |  | 1..1 | groep |  |
| &emsp;**`BrAlg`** | Bericht algemeen | 1..1 | groep |  |
| &emsp;&emsp;`BrCd` | Bericht, code | 1..1 | an..5 | 00703 |
| &emsp;&emsp;`VnrBrCd` | Versienummer bericht, code | 1..1 | an..5 | 00002 |
| &emsp;&emsp;`AandatBr` | Aanmaakdatum bericht | 1..1 | datum |  |
| &emsp;&emsp;`AantijdBr` | Aanmaaktijd bericht | 1..1 | tijd |  |
| &emsp;&emsp;`IdInzndr` | Identificatie inzender | 1..1 | an..40 |  |
| &emsp;&emsp;`GebrSwPakket` | Gebruikt softwarepakket | 1..1 | an..35 |  |
| &emsp;&emsp;`IdOntvngr` | Identificatie ontvanger | 1..1 | an..40 |  |
| &emsp;&emsp;`Berrefnr` | Berichtreferentienummer | 1..1 | an..512 |  |
| &emsp;&emsp;`TestJN` | Test J/N | 1..1 | an1 | J, N, O |
| &emsp;&emsp;`OntvngstbevJN` | Ontvangstbevestiging gewenst J/N | 1..1 | an1 | J, N, O |
| &emsp;**`VrzkrVolmacht`** | Verzekeraar/volmacht | 0..1 | groep |  |
| &emsp;&emsp;`HndlsnmOrg` | Handelsnaam organisatie | 1..1 | an..100 |  |
| &emsp;&emsp;`IdVrzkrVolmachtCd` | Identificatie verzekeraar/volmacht, code | 1..1 | an..4 |  |
| &emsp;**`Arbdnst`** | Arbodienst | 0..1 | groep |  |
| &emsp;&emsp;`HndlsnmOrg` | Handelsnaam organisatie | 1..1 | an..100 |  |
| &emsp;&emsp;`ArbdnstCd` | Arbodienst, code | 0..1 | an3 |  |
| &emsp;**`Verslagperiode`** | Verslagperiode | 1..999 | groep |  |
| &emsp;&emsp;`Ingdat` | Ingangsdatum | 1..1 | datum |  |
| &emsp;&emsp;`Enddat` | Einddatum | 1..1 | datum |  |
| &emsp;&emsp;**`Rapportage`** | Rapportage | 1..1 | groep |  |
| &emsp;&emsp;&emsp;`AantalKlanten` | Aantal klanten | 1..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalMeldingen` | Aantal werknemers | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalVerzuimmeldingen` | Aantal verzuimmeldingen | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalVerzuimdagen` | Aantal verzuimdagen | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`Verzuimpercentage` | Verzuimpercentage | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`Verzuimfrequentie` | Verzuimfrequentie | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalDeelherstelmeldingen` | Aantal deelherstelmeldingen | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentageDeelherstelmeldingen` | Percentage deelherstelmeldingen | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`AantalHerstelmeldingen` | Aantal herstelmeldingen | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentageHerstelmeldingen` | Percentage herstelmeldingen | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`AantalMeldingenRegres` | Aantal meldingen regres | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`GemiddeldeVerzuimduur` | Gemiddelde verzuimduur (gesloten dossiers) | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`ZiekteverzuimpercentageKort` | Ziekteverzuimpercentage 1-7 dgn | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`ZiekteverzuimpercentageMiddellang` | Ziekteverzuimpercentage 8-42 dgn | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`ZiekteverzuimpercentageLang` | Ziekteverzuimpercentage 43-365 dgn | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`ZiekteverzuimpercentageExtraLang` | Ziekteverzuimpercentage >365 dgn | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`AantalMeldingenVerzuimKort` | Aantal meldingen verzuim 1-7 werkdagen | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalMeldingenVerzuimMiddellang` | Aantal meldingen verzuim  8-42 werkdagen | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalMeldingenVerzuimLang` | Aantal meldingen verzuim 43-365 werkdagen | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalMeldingenVerzuimExtraLang` | Aantal meldingen verzuim > 365 dagen | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalZiekdagenKort` | Aantal ziekdagen 1-7 werkdagen | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalZiekdagenMiddellang` | Aantal ziekdagen 8-42 werkdagen | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalZiekdagenLang` | Aantal ziekdagen  43-365 werkdagen | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalZiekdagenExtraLang` | Copyright SIVI | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalProbleemanalysesOpgesteld` | Aantal probleemanalyses opgesteld | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentageProbleemanalysesOpTijd` | Percentage probleemanalyses op tijd | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`AantalPlannenVanAanpakOpgesteld` | Aantal plannen van aanpak opgesteld | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentagePlannenVanAanpakOpTijd` | Percentage plannen van aanpak op tijd | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`AantalTweeenveertigWeeksmeldingenGedaan` | Aantal 42 weeksmeldingen gedaan | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentageTweeenveertigWeeksmeldingenOpTijd` | Percentage 42 weeksmeldingen op tijd | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`AantalEindejaarsevaluatiesGedaan` | Aantal eindejaarsevaluaties gedaan | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentageEindejaarsevaluatiesOpTijd` | Percentage eindejaarsevaluaties op tijd | 0..1 | n..6,2 |  |
| &emsp;&emsp;&emsp;`AantalReintegratieverslagenOpgesteld` | Aantal re-integratieverslagen opgesteld | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentageReintegratieverslagenOpTijd` | Percentage re-integratieverslagen op tijd | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalPoortwachtersancties` | Aantal poortwachtersancties | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalGeadviseerdeInterventies` | Aantal geadviseerde interventies | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalGeaccordeerdeInterventies` | Aantal geaccordeerde interventies | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalInterventiesMetBijdrageVerzekeraar` | Aantal interventies met bijdrage Verzekeraar | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`KostenInterventiesVootVerzekeraar` | Kosten interventies voor Verzekeraar | 0..1 | n..9,2 |  |
| &emsp;&emsp;&emsp;`AantalTweedeSpoor` | Aantal tweede spoor | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalPsychischeInterventies` | Aantal  psychische interventies | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalFysiekeInterventies` | Aantal fysieke interventies | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalMultidisciplinaireInterventies` | Aantal multidisciplinaire interventies | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalWachtlijstbemiddelingen` | Aantal wachtlijstbemiddelingen | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalOverigeInterventies` | Aantal overige internventies | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`Werkgevertevredenheid` | Werkgevertevredenheid van 0 - 10 | 0..1 | n..3 |  |
| &emsp;&emsp;&emsp;`AantalGemeldeKlachten` | Aantal gemelde klachten | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`AantalTerechteKlachten` | Aantal terechte klachten | 0..1 | n..7 |  |
| &emsp;&emsp;&emsp;`PercentageTerechteKlachten` | Copyright SIVI | 0..1 | n..6,2 |  |
