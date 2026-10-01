# SIVI Verzuim: Arbodiensten ↔ Verzekeraars

Specificatie en documentatie voor gegevensuitwisseling tussen Arbodiensten en Inkomensverzekeraars / Volmachten.

---

### De SIVI Verzuim Driehoek (Model B)

De SIVI Verzuimstandaard verbindt de drie hoofdrolspelers in de verzuimbegeleiding en inkomensverzekering via drie afzonderlijk beheerde maar inhoudelijk consistente koppelvlakken:

```
                  ┌───────────────────────────────┐
                  │          WERKGEVERS           │
                  │   (HR & Salarissoftware)      │
                  └──────────────┬────────────────┘
                                 │
                 Koppelvlak 1    │    Koppelvlak 2
                 (Arbodienst)    │    (Verzekering)
                                 │
           ┌─────────────────────┴─────────────────────┐
           ▼                                           ▼
┌───────────────────────────────┐             ┌───────────────────────────────┐
│         ARBODIENSTEN          │◄───────────►│         VERZEKERAARS          │
│     (Arbodienstsystemen)      │ Koppelvlak 3│  (Inkomensverzekeraars/Volm.) │
└───────────────────────────────┘             └───────────────────────────────┘
```

> [!NOTE] Drie gescheiden repositories voor doelgroepgerichte helderheid
> Elk koppelvlak heeft een eigen GitHub repository met eigen documentatie, issues, discussies en XSD-releaseschema's:
> 
> 1. **[Werkgevers ↔ Arbodiensten](https://ducosivi.github.io/sim-verzuim-werkgevers-arbodiensten/)** &mdash; Focus op verzuimregistratie, re-integratie en Poortwachter.
> 2. **[Werkgevers ↔ Verzekeraars](https://ducosivi.github.io/sim-verzuim-werkgevers-verzekeraars/)** &mdash; Focus op polisdekking, loonaangifte en schadeclaims.
> 3. **[Arbodiensten ↔ Verzekeraars](https://ducosivi.github.io/sim-verzuim-arbodiensten-verzekeraars/)** &mdash; Focus op interventies, voortgang en privacy-conforme afstemming.

---

## Doel en Toepassingsgebied

Dit koppelvlak faciliteert de afstemming over re-integratietrajecten, interventies en WIA-voorbereiding met strikte naleving van de medische privacy (AVG).

Belangrijke karakteristieken van dit koppelvlak:
* **Focus:** Aanvragen en toekennen van interventiebudgetten, Poortwachter-mijlpalen en procesmatige herstelprognoses (uitsluitend functionele mogelijkheden).
* **Gemeenschappelijke kern:** Maakt gebruik van de uniforme SIVI-bouwstenen voor werknemer-, werkgever- en verzuimidentificatie.
* **Gegevensminimalisatie:** Strikt afgestemd op de wettelijke bevoegdheden en de AVG-kaders van de betrokken partijen.

---

## Direct aan de slag

* Raadpleeg de [Bedrijfsprocessen](processen.md) voor de trigger- en informatiestromen.
* Bekijk de [Berichtenspecificatie](berichten.md) en download de schema's uit de map `schema/`.
* Bekijk de geldige waardes in de [Codelijsten](codelijsten.md).
* Lees de [Implementatiehandleiding](implementatie.md) voor validatieregels en testscenario's.
