# Literaturrecherche Diskussion/Handlungsempfehlungen — Gesundheitsbericht Kolonkarzinom

**Kontext:** Sterbefälle infolge bösartiger Neubildungen des Kolons (ICD-10 C18–C21), Deutschland vs. NRW vs. Bayern, 2014–2024, Alter 50–95+, nach Geschlecht. Hauptergebnisse: (1) Sterblichkeit sinkt 2014–2024, (2) NRW durchgängig höher als Bayern/Deutschland, (3) starker Altersgradient, (4) Männer > Frauen.

**Recherche-Session:** 2026-08-16, Claude Code Remote (Branch `claude/kolonkarzinom-literatur-recherche-8nq28x`).

---

## ⚠️ Verifikationsstatus — bitte zuerst lesen

Die Remote-Session hatte eine **Netzwerk-Sperre**: Kein einziger externer Dokumentabruf war möglich (rki.de, edoc.rki.de, gbe.rki.de, doi.org, versorgungsatlas.de, PubMed Central — alle blockiert). Erreichbar waren nur **Websuche** und **GitHub**.

Jede Angabe unten trägt daher eines von drei Labels:

| Label | Bedeutung |
|---|---|
| ✅ **VERIFIZIERT (Dokument geöffnet)** | Wert/Zitat wurde direkt in der geöffneten Originaldatei gelesen (nur bei der RKI-GitHub-Datenquelle möglich). |
| 🔶 **SUCH-VERIFIZIERT** | Exakt-Phrasen-Suche: Der exakte String (DOI, Titel, Autorenliste) wurde als Suchbegriff verwendet und lieferte Treffer auf der offiziellen Domain. Sehr zuverlässig für Metadaten, aber kein Ersatz für das geöffnete Dokument. |
| ❌ **NICHT VERIFIZIERT** | Stammt nur aus Suchmaschinen-Snippets. NICHT in den Bericht übernehmen, bevor die Heimmaschine es geprüft hat. |

**→ Alle mit `[ ]` markierten Prüfpunkte werden von der Heimmaschine abgearbeitet** (siehe `UEBERGABE_PROMPT_heimmaschine.md`).

---

## Quelle 0 (PFLICHT erledigt): Starker et al. 2017 — DOI + Autorenkorrektur

**APA 7:** 🔶
> Starker, A., Buttmann-Schweiger, N., Kraywinkel, K., & Kuhnert, R. (2017). Inanspruchnahme der Darmspiegelung in Deutschland. *Journal of Health Monitoring, 2*(4), 81–87. https://doi.org/10.17886/RKI-GBE-2017-115

**DOI:** `10.17886/RKI-GBE-2017-115` 🔶 — zweifach such-verifiziert:
1. Exakt-Suche `"10.17886/RKI-GBE-2017-115"` → Treffer u. a. auf krebsdaten.de (RKI, „Fachpublikationen 2017") und edoc.rki.de.
2. Exakt-Suche `"Inanspruchnahme der Darmspiegelung in Deutschland" "Starker" "81" "2017"` → Treffer: edoc.rki.de/handle/176904/2904 (Landing Page + PDF), rki.de-Fact-Sheet-Seite, gbe.rki.de.

**⚠️ AUTORENKORREKTUR gegenüber Übergabe-Brief:** Nicht „Starker, Bertz, Saß" — die korrekte Autorenliste ist **Starker, Buttmann-Schweiger, Kraywinkel, Kuhnert**. („Starker/Bertz/Saß" gehört zu einer anderen Publikation über Krebsfrüherkennungsuntersuchungen.)

**Direkte RKI-Links (alle 🔶, von der Session nicht öffenbar):**
- Landing Page: https://edoc.rki.de/handle/176904/2904
- PDF (Volltext, CC BY): https://edoc.rki.de/bitstream/handle/176904/2904/22s1e1tx0Baw.pdf
- RKI-Fact-Sheet-Seite: https://www.rki.de/DE/Aktuelles/Publikationen/Journal-of-Health-Monitoring/GBEDownloadsJ/FactSheets/JoHM_04_2017_Darmspiegelung.html
- GBE-Seite: https://www.gbe.rki.de/SharedDocs/Publikationen/DE/Starker-2017-Inanspruchnahme-Darmkrebsvorsorge.html
- Englische Fassung (separater DOI `10.17886/RKI-GBE-2017-126`): https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10165909/

**Kernaussage-Kandidat** ❌ (aus Suchsnippet, Wortlaut prüfen): Rund 57 % der Frauen und 61 % der Männer ab 55 Jahren berichten eine Darmspiegelung in den letzten 10 Jahren.

**Prüfpunkte Heimmaschine:**
- [ ] `https://doi.org/10.17886/RKI-GBE-2017-115` aufrufen → muss auf edoc.rki.de/handle/176904/2904 auflösen.
- [ ] Autorenliste auf S. 81 des PDF gegenlesen.
- [ ] Wortlaut + Seitenzahl der Kernaussage (Frauen/Männer-Anteile, vermutlich S. 81 Abstract oder S. 83) aus dem PDF ziehen.

**Dient im Bericht:** Beleg für geschlechtsspezifische Inanspruchnahme der Darmspiegelung (Diskussion Männer > Frauen). *(War bereits in Teil A gesichert — hier nur DOI-Nachtrag + Autorenkorrektur.)*

---

## Quelle 1 (C2): Zi-Versorgungsatlas — regionale Unterschiede der Screening-Teilnahme

**APA 7:** 🔶
> Steffen, A., Holstiege, J., Hagen, B., Akmatov, M. K., & Bätzing, J. (2020). *Inanspruchnahme der Darmkrebsfrüherkennung in den Jahren 2009 bis 2018: Eine Bestandsaufnahme auf Basis bundesweiter vertragsärztlicher Abrechnungsdaten* (Versorgungsatlas-Bericht Nr. 20/02). Zentralinstitut für die kassenärztliche Versorgung in Deutschland (Zi). https://doi.org/10.20364/VA-20.02

**DOI:** `10.20364/VA-20.02` 🔶 — Exakt-Suche `"10.20364/VA-20.02" Darmkrebsfrüherkennung` → Treffer: versorgungsatlas.de (PDF + Landing Page), zi.de-Pressemitteilung 14.05.2020, ResearchGate.

**Links (🔶, frei zugänglich laut Zi-Publikationspraxis):**
- PDF: https://www.versorgungsatlas.de/fileadmin/ziva_docs/108/VA_Bericht_20-02_Darmkrebsfr%C3%BCherkennung_2020-05-14.pdf
- Landing Page: https://www.versorgungsatlas.de/themen/alle-analysen-nach-datum-sortiert/108/einleitung/
- Zi-Pressemitteilung (14.05.2020): https://www.zi.de/detailansicht/14-mai-2020

**Inhaltliche Kandidaten** ❌ (aus Snippets/Pressemitteilung, Wortlaut prüfen):
- Jährliche Teilnahmequoten an der präventiven Darmspiegelung stagnieren bei ca. 2,5 % (Titel der Zi-Pressemitteilung: „Teilnahme an Darmkrebsfrüherkennung weiter ausbaufähig – Jährliche Teilnahmequoten an präventiver Darmspiegelung stagnieren bei 2,5 Prozent").
- Deutliche regionale Variation der Inanspruchnahme; Auswertung nach KV-Regionen (Achtung: NRW = KV Nordrhein + KV Westfalen-Lippe getrennt) und Kreisen.

**Prüfpunkte Heimmaschine:**
- [ ] PDF öffnen, aus der Zusammenfassung (erwartet S. 3–4) 1–2 wörtliche Sätze zur regionalen Variation ziehen (Suchwort im PDF: „regional").
- [ ] Konkrete Teilnahmeraten für KV Nordrhein, KV Westfalen-Lippe und KV Bayerns aus den Abbildungen/Tabellen notieren (Suchwort: „Nordrhein", „Bayern").
- [ ] Prüfen, ob NRW-Werte tatsächlich über den bayerischen liegen — NICHT vorab annehmen.

**Dient im Bericht:** Zweite Erklärung (neben Deprivation, Hoebel et al. 2024) für NRW > Bayern: regional unterschiedliche Screening-Inanspruchnahme; zugleich Basis der Handlungsempfehlung „Teilnahme steigern".

---

## Quelle 2 (C3): RKI/GEDA — Risikofaktoren-Prävalenz NRW vs. Bayern

**APA 7:** ✅ (Datensatz direkt geöffnet)
> Robert Koch-Institut. (2026). *Gesundheitsberichterstattung – Daten zu nichtübertragbaren Erkrankungen* (Version 2026-07-15) [Datensatz]. Zenodo. https://doi.org/10.5281/zenodo.13736662

Lizenz CC BY 4.0. Datengrundlage der Werte: GEDA 2019/2020-EHIS (telefonische Befragung, N = 23.001, ab 18 Jahren). Maschinenlesbare Grundlage der GBE-Webseite gbe.rki.de.

**Links:**
- GitHub (✅ geöffnet): https://github.com/robert-koch-institut/Gesundheitsberichterstattung_-_Daten_zu_nichtuebertragbaren_Erkrankungen — Datei `GBE_Indikatoren_nichtuebertragbarer_Erkrankungen.tsv`
- Interaktiv (🔶): https://www.gbe.rki.de/adipositas-und-uebergewicht · https://www.gbe.rki.de/rauchen

**Kernaussage 1** ✅ (wörtlich aus Readme.md des Datensatzes, Abschnitt „Indikator ‚Darmkrebs: Sterblichkeit'", Zeile 4499; Linktexte entfernt):
> „Zu den wichtigsten beeinflussbaren Risikofaktoren für Darmkrebs gehören Rauchen und Adipositas, gefolgt von Bewegungsmangel, ballaststoffarmer Ernährung, Alkoholkonsum und häufiger Verzehr von rotem beziehungsweise verarbeitetem Fleisch."

**Kernaussage 2 — Zahlen NRW vs. Bayern** ✅ (TSV, Indikatoren `2060201` Rauchen / `1020501` Adipositas, Berichtsjahr 2019, ab 18 Jahre, Gesamt, altersstandardisiert Europastandard 2013, 95-%-KI):
| Indikator | NRW | Bayern | Deutschland |
|---|---|---|---|
| Rauchen (täglich/gelegentlich) | **31,2 %** (28,9–33,6) | **26,6 %** (24,2–29,1) | 29,6 % |
| Adipositas (BMI ≥ 30) | **19,7 %** (17,9–21,6) | **18,0 %** (15,9–20,2) | 18,8 % |

**Formulierungshinweise (Statistik):**
- Rauchen: 95-%-KIs überlappen kaum → als robusten Unterschied darstellbar.
- Adipositas: KIs überlappen deutlich → nur als „tendenziell höher" formulieren.
- ⚠️ **Gegenrichtung Alkohol:** „moderates bis hohes Risiko" in Bayern (37,4 %) höher als NRW (31,4 %) — Alkohol NICHT als NRW-Erklärung verwenden.
- Kontext Bewegung (Ausdauerempfehlung erreicht): NRW 48,5 % vs. Bayern 51,2 % (konsistent, kleiner Unterschied).

**Prüfpunkte Heimmaschine:**
- [ ] Optional: klassischen Journal-Beleg ergänzen (z. B. Schienkiewitz et al., JoHM 3/2022 zu Übergewicht/Adipositas, oder aktuelle GEDA-Publikation) und dessen Bundesland-Werte gegen die TSV prüfen — falls der Kurs Datensatz-Zitationen nicht akzeptiert.
- [ ] DOI `10.5281/zenodo.13736662` auflösen und Versionsstand prüfen.

**Dient im Bericht:** Ergänzende Erklärung für NRW > Bayern über verhaltensbezogene Risikofaktoren (Rauchen deutlich, Adipositas tendenziell häufiger in NRW).

---

## Quelle 3 (C4): Wirksamkeit von Einladungsverfahren

Zwei Kandidaten — **Empfehlung: 3a (Gruner) als Hauptbeleg** wegen Deutschland-Bezug, 3b (Green) als sofort zitierfähige Alternative.

### 3a — Gruner et al. 2020 (Deutschland, RCT) — BEVORZUGT

**APA 7:** 🔶 (Zitation wörtlich verifiziert über die Referenzliste eines geöffneten Open-Access-Volltexts, BMC Medicine 2025, DOI 10.1186/s12916-025-03948-9)
> Gruner, L. F., Hoffmeister, M., Ludwig, L., Meny, S., & Brenner, H. (2020). The effects of differing invitation models on the uptake of immunological fecal occult blood testing. *Deutsches Ärzteblatt International, 117*(25), 423–430. https://doi.org/10.3238/arztebl.2020.0423

DKFZ-Gruppe (Brenner/Hoffmeister); dreiarmige RCT, 17.532 AOK-Baden-Württemberg-Versicherte, 50–54 Jahre.

**Links (🔶, laut Suchtreffern open access):**
- PMC (englisch): https://pmc.ncbi.nlm.nih.gov/articles/PMC7490457/ (PMID 32885780)
- Deutsches Ärzteblatt (deutsch): https://aerzteblatt.de/archiv/214401

**Kerndaten** ❌ (nur aus konsistenten Such-Snippets — Wortlaut zwingend prüfen): FIT-Nutzung binnen eines Jahres ca. 29,7 % (Einladung mit beigelegtem Test) bzw. 27,7 % (Einladung mit Anforderungsoption) vs. ca. 10 % Kontrollgruppe (nur Anschreiben) — grob eine Verdreifachung (+18–20 Prozentpunkte).

**Prüfpunkte Heimmaschine:**
- [ ] PMC7490457 öffnen, die Teilnahmeraten aller drei Arme wörtlich aus dem Abstract (Results) mit Fundstelle ziehen.
- [ ] DOI `10.3238/arztebl.2020.0423` auflösen.

**Dient im Bericht:** Direktester deutscher RCT-Beleg für die Handlungsempfehlung „Teilnahme steigern": Persönliche Einladung mit beigelegtem/leicht anforderbarem Stuhltest erhöht die Screening-Teilnahme drastisch.

### 3b — Green et al. 2022 (USA, RCT, 9 Jahre) — Alternative, bereits wörtlich belegt

**APA 7:** ✅ (Volltext-XML des PMC-Artikels über GitHub-Mirror geöffnet und gelesen)
> Green, B. B., Anderson, M. L., Cook, A. J., Chubak, J., Fuller, S., Meenan, R. T., & Vernon, S. W. (2022). A centralized program with stepped support increases adherence to colorectal cancer screening over 9 years: A randomized trial. *Journal of General Internal Medicine, 37*(5), 1073–1080. https://doi.org/10.1007/s11606-021-06922-2

**Link:** https://pmc.ncbi.nlm.nih.gov/articles/PMC8162159/ (PMCID PMC8162159; gelesenes XML: https://raw.githubusercontent.com/choxos/funded-trials/main/pmc_nih/PMC%208162159.xml)

**Kernaussage 1** ✅ (Abstract, Key Results; UC = usual care):
> "Compared to UC, intervention participants had 21% more covered time over 9 years (57.5% vs. 69.1%; adjusted incidence rate ratio 1.21, 95% confidence interval 1.16–1.25, P < 0.001)."

**Kernaussage 2** ✅ (Abstract, Conclusions):
> "An outreach program that included mailed fecal tests and phone follow-up led to increased adherence to CRC testing and fewer age-eligible individuals without any CRC testing over 9 years."

**Dient im Bericht:** Randomisierter Langzeit-Beleg, dass organisiertes Einladungs-/Outreach-Programm (postalische Stuhltests + Erinnerungen) die dauerhafte Screening-Teilnahme signifikant erhöht — sofort zitierfähig, falls 3a nicht verifiziert werden kann.

---

## Empfehlung zur Übernahme (max. 3–4 neue Quellen)

1. **Steffen et al. 2020 (Versorgungsatlas 20/02)** — regionale Screening-Unterschiede (nach Heimmaschinen-Prüfung).
2. **RKI-GEDA-Datensatz 2026 (bzw. ersatzweise eine JoHM-Publikation dazu)** — Risikofaktoren NRW vs. Bayern (Zahlen bereits verifiziert).
3. **Gruner et al. 2020 (Dtsch Arztebl Int)** — Einladungsverfahren/Handlungsempfehlung (nach Heimmaschinen-Prüfung; sonst ersatzweise Green et al. 2022, bereits wörtlich belegt).

Der Starker-DOI ist kein Neuzugang, sondern Nachtrag zu Teil A. Damit bleibt das Budget (~8.400 Zeichen Diskussion) eingehalten.
