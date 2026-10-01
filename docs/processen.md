# Bedrijfsprocessen: Arbodiensten ↔ Verzekeraars

Dit document beschrijft de gegevensuitwisseling tussen arbodiensten en verzekeraars met betrekking tot re-integratie en interventies.

---

## 1. Aanvraag Interventie (Schadelastbeheersing)
* **Trigger:** Bedrijfsarts adviseert een gerichte interventie (bijv. psychologische ondersteuning, werkplekaanpassing, fysiotherapie).
* **Actie arbodienst:** Verzending van `InterventieAanvraag` met omschrijving van het interventiedoel, offerte van de interventiepartij en verwachte verkorting van de verzuimduur.
* **Actie verzekeraar:** Beoordeling op dekking binnen de polis (preventie- of interventiebudget) en terugkoppeling van akkoordverklaring.

## 2. Voortgang Re-integratiestatus (Poortwachter)
* **Trigger:** Bereiken van wettelijke mijlpalen (week 6 Probleemanalyse, week 52 Eerstejaarsevaluatie, week 88 WIA-aanvraag).
* **Actie arbodienst:** Verzending van `ReintegratieStatus` met procesmatige status en prognose (uitsluitend functionele capaciteiten, GEEN medische diagnosen).
* **Actie verzekeraar:** Monitoring van het Poortwachter-risico en tijdige ondersteuning bij re-integratie tweede spoor.
