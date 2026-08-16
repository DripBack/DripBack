# Literaturrecherche Diskussion/Handlungsempfehlungen — Gesundheitsbericht Kolonkarzinom

**Kontext:** Sterbefälle infolge bösartiger Neubildungen des Kolons (ICD-10 C18–C21), Deutschland vs. NRW vs. Bayern, 2014–2024, Alter 50–95+, nach Geschlecht. Hauptergebnisse: (1) Sterblichkeit sinkt 2014–2024, (2) NRW durchgängig höher als Bayern/Deutschland, (3) starker Altersgradient, (4) Männer > Frauen.

**Recherche-Session:** 2026-08-16, Claude Code Remote (Branch `claude/kolonkarzinom-literatur-recherche-8nq28x`).
**Heimmaschinen-Verifikation:** 2026-08-16 — alle PDFs geöffnet, Zitate wörtlich gegengelesen, C4 ergänzt (inkl. des vom Remote-Agenten nachgeschobenen Gruner-Kandidaten).

---

## ⚠️ Verifikationsstatus — bitte zuerst lesen

Die Remote-Session hatte eine **Netzwerk-Sperre**; die Heimmaschine hat am 2026-08-16 alle offenen Punkte mit echtem Dokumentabruf abgearbeitet.

| Label | Bedeutung |
|---|---|
| ✅ **VERIFIZIERT (Dokument geöffnet)** | Wert/Zitat wurde direkt in der geöffneten Originaldatei gelesen. |
| 🔶 **SUCH-VERIFIZIERT** | Nur Exakt-Phrasen-Suche (Metadaten-Treffer auf offizieller Domain), Dokument nicht geöffnet. |
| ❌ **NICHT VERIFIZIERT** | Nur Suchmaschinen-Snippet. Nicht in den Bericht übernehmen. |

**Stand nach Heimmaschinen-Lauf: keine ❌- oder 🔶-Angaben mehr in den übernommenen Kernaussagen.**

---

## Quelle 0 (PFLICHT erledigt): Starker et al. 2017 — DOI + Autorenkorrektur

**APA 7:** ✅ (PDF geöffnet, Impressum S. 87 „Zitierweise“ gegengelesen)
> Starker, A., Buttmann-Schweiger, N., Kraywinkel, K., & Kuhnert, R. (2017). Inanspruchnahme der Darmspiegelung in Deutschland. *Journal of Health Monitoring, 2*(4), 81–87. https://doi.org/10.17886/RKI-GBE-2017-115

**DOI:** `10.17886/RKI-GBE-2017-115` ✅ — am 2026-08-16 über doi.org aufgelöst: landet mit HTTP 200 auf `https://edoc.rki.de/handle/176904/2904`. PDF von dort geladen (7 Seiten, 73 KB, CC BY).

**✅ AUTORENKORREKTUR bestätigt (S. 81, Kopfspalte „Autorinnen und Autoren“):** Anne Starker, Nina Buttmann-Schweiger, Klaus Kraywinkel, Ronny Kuhnert. („Starker/Bertz/Saß“ aus dem Übergabe-Brief gehört zu einer anderen Publikation; die DEGS1-Arbeit „Starker & Saß 2013“ wird im Fact Sheet selbst als Referenz 9 zitiert.)

**Direkte RKI-Links (✅ funktionieren):**
- Landing Page: https://edoc.rki.de/handle/176904/2904
- PDF (Volltext, CC BY): https://edoc.rki.de/bitstream/handle/176904/2904/22s1e1tx0Baw.pdf

**Kernaussagen ✅ (wörtlich aus dem geöffneten PDF):**
- Abstract, S. 81: „57 % der Frauen und 61 % der Männer im Alter ab 55 Jahren gaben an, dass bei ihnen innerhalb der letzten 10 Jahre eine Darmspiegelung durchgeführt wurde.“
- Präzise Werte, S. 83 („Ergebnisse und Einordnung“): „In Deutschland geben laut GEDA 2014/2015-EHIS-Daten 56,5 % der Frauen und 60,8 % der Männer ab 55 Jahren an, dass bei ihnen innerhalb der letzten 10 Jahre eine Darmspiegelung durchgeführt wurde“.
- Geschlechtervergleich, S. 83: „Im Geschlechtervergleich fällt auf, dass in der Altersgruppe der 70-Jährigen und Älteren der Anteil der Männer, bei denen innerhalb der letzten 10 Jahre eine Darmspiegelung durchgeführt wurde, größer ist als bei den Frauen.“ (Tabelle 1, S. 84: ≥ 70 Jahre Männer 67,5 % vs. Frauen 59,1 %.)

**⚠️ Richtungs-Hinweis für die Diskussion:** Bei der *Darmspiegelung* berichten Männer ab 55 höhere Inanspruchnahme als Frauen — die Aussage „Männer nehmen Vorsorge seltener wahr“ gilt nur für den *Stuhltest* (siehe Steffen et al. 2020 und Hoffmeister et al. 2017), nicht pauschal.

**Prüfpunkte Heimmaschine:**
- [x] `https://doi.org/10.17886/RKI-GBE-2017-115` aufrufen → löst auf edoc.rki.de/handle/176904/2904 auf (HTTP 200, verifiziert 2026-08-16).
- [x] Autorenliste auf S. 81 des PDF gegengelesen (Starker, Buttmann-Schweiger, Kraywinkel, Kuhnert).
- [x] Wortlaut + Seitenzahl der Kernaussage gezogen (Abstract S. 81; präzise Werte S. 83; Tabelle 1 S. 84).

**Dient im Bericht:** Beleg für geschlechtsspezifische Inanspruchnahme der Darmspiegelung (Diskussion Männer > Frauen — mit obigem Richtungs-Hinweis). *(War bereits in Teil A gesichert — hier DOI-Nachtrag + Autorenkorrektur.)*

---

## Quelle 1 (C2): Zi-Versorgungsatlas — regionale Unterschiede der Screening-Teilnahme

**APA 7:** ✅ (PDF geöffnet, „Zitierweise“ S. 2 gegengelesen)
> Steffen, A., Holstiege, J., Hagen, B., Akmatov, M. K., & Bätzing, J. (2020). *Inanspruchnahme der Darmkrebsfrüherkennung in den Jahren 2009 bis 2018: eine Bestandsaufnahme auf Basis bundesweiter vertragsärztlicher Abrechnungsdaten* (Versorgungsatlas-Bericht Nr. 20/02). Zentralinstitut für die kassenärztliche Versorgung in Deutschland (Zi). https://doi.org/10.20364/VA-20.02

**DOI:** `10.20364/VA-20.02` ✅ — am 2026-08-16 aufgelöst auf `https://www.versorgungsatlas.de/themen/alle-analysen-nach-datum-sortiert/108/einleitung/` (HTTP 200). PDF frei geladen (26 Seiten, 4,4 MB).

**Links (✅ funktionieren):**
- PDF: https://www.versorgungsatlas.de/fileadmin/ziva_docs/108/VA_Bericht_20-02_Darmkrebsfr%C3%BCherkennung_2020-05-14.pdf
- Landing Page: https://www.versorgungsatlas.de/themen/alle-analysen-nach-datum-sortiert/108/einleitung/

**Kernaussagen ✅ (wörtlich aus dem geöffneten PDF):**
- Zusammenfassung/Ergebnisse, S. 1–2: „Die Inanspruchnahme der präventiven Koloskopie blieb stabil mit jährlich rund 2,6 % bei Frauen und 2,5 % bei Männern in der primären Zielgruppe der 55- bis 64-Jährigen.“
- Zusammenfassung/Ergebnisse, S. 2: „Die regionale Variation in der Inanspruchnahme ist sowohl auf Jahresebene als auch über den 10-Jahres-Zeitraum hoch, doch wird sie teilweise durch den unterschiedlichen Einsatz kurativer Koloskopien abgeschwächt.“
- Schlussfolgerung, S. 2: „Die Teilnahme an den Angeboten der darmkrebsbezogenen Früherkennung ist weiter ausbaufähig und variiert deutlich zwischen den Regionen.“
- Kernaussagen-Kasten, S. 4: „Die Inanspruchnahme von Angeboten der darmkrebsbezogenen Früherkennung ist von starker regionaler Variation gekennzeichnet.“

**Teilnahmeraten KV Nordrhein / KV Westfalen-Lippe / KV Bayerns** ✅ (Tabelle 2, S. 15 — 10-Jahres-Inanspruchnahme der Kohorte, die 2009 55 Jahre alt war, Angaben in Prozent):

| KV-Bereich | Präv. Koloskopie (F) | Präv. Koloskopie (M) | Präv. Koloskopie oder ≥3 FOBT (F) | Präv. Koloskopie oder ≥3 FOBT (M) |
|---|---|---|---|---|
| Bayerns | 27,6 | 27,6 | 45,1 | 34,5 |
| Nordrhein | 25,5 | 25,3 | 44,9 | 35,6 |
| Westfalen-Lippe | 24,5 | 24,4 | 44,7 | 34,9 |

**Ergebnisoffene Prüfung (Auftrag: „liegen die NRW-Regionen wirklich über Bayern?“) — Ergebnis:**
- Bei der **präventiven Koloskopie liegen beide NRW-KVs UNTER Bayern** (Differenz 2–3 Prozentpunkte, beide Geschlechter). Das ist die für die NRW-Erklärung passende Richtung (geringere Screening-Teilnahme ↔ höhere Sterblichkeit), aber der Abstand ist klein.
- Beim kombinierten Maß „Vorsorge gemäß KFE-RL“ (präventive Koloskopie oder ≥3 FOBT) sind die drei KVs **praktisch gleichauf** (Frauen: Bayern minimal vorn; Männer: Nordrhein minimal vorn).
- **Formulierungsempfehlung:** Die Zi-Daten belegen *starke regionale Variation insgesamt* und eine *insgesamt ausbaufähige Teilnahme*; als Beleg für „NRW screent deutlich weniger als Bayern“ taugen sie nur eingeschränkt (kleiner Unterschied nur bei der präventiven Koloskopie). Nicht überinterpretieren.
- Jahresbezogene KV-Werte stehen im Bericht nur als Abbildungen (Abb. 4 FOBT, Abb. 6 präventive Koloskopie) ohne Zahlenbeschriftung; belastbare Zahlen daher aus Tabelle 2 (S. 15).

**Prüfpunkte Heimmaschine:**
- [x] PDF geöffnet, wörtliche Sätze zur regionalen Variation aus der Zusammenfassung gezogen (S. 2, s. o.).
- [x] Konkrete Teilnahmeraten für KV Nordrhein, KV Westfalen-Lippe und KV Bayerns notiert (Tabelle 2, S. 15).
- [x] Ergebnisoffen geprüft: NRW liegt bei präventiver Koloskopie UNTER Bayern (klein); beim KFE-RL-Gesamtmaß nahezu gleichauf — klar vermerkt, s. o.

**Dient im Bericht:** Zweite Erklärung (neben Deprivation, Hoebel et al. 2024) für NRW > Bayern: regional unterschiedliche Screening-Inanspruchnahme (vorsichtig formuliert, s. Prüfergebnis); zugleich Basis der Handlungsempfehlung „Teilnahme steigern“.

---

## Quelle 2 (C3): RKI/GEDA — Risikofaktoren-Prävalenz NRW vs. Bayern

**APA 7:** ✅ (Datensatz direkt geöffnet; Version aktualisiert nach DOI-Auflösung 2026-08-16)
> Robert Koch-Institut. (2026). *Gesundheitsberichterstattung – Daten zu nichtübertragbaren Erkrankungen* (Version 2026-07-15) [Datensatz]. Zenodo. https://doi.org/10.5281/zenodo.13736662

Lizenz CC BY 4.0. Datengrundlage der Werte: GEDA 2019/2020-EHIS (telefonische Befragung, N = 23.001, ab 18 Jahren). Maschinenlesbare Grundlage der GBE-Webseite gbe.rki.de.

**Links:**
- GitHub (✅ geöffnet): https://github.com/robert-koch-institut/Gesundheitsberichterstattung_-_Daten_zu_nichtuebertragbaren_Erkrankungen — Datei `GBE_Indikatoren_nichtuebertragbarer_Erkrankungen.tsv`
- Zenodo-Version 2026-07-15 (✅): https://zenodo.org/records/21242132
- Interaktiv (✅ geöffnet): https://www.gbe.rki.de/rauchen — statische Seite nennt DE-weit 28,9 % Rauchen 2019 (rohe Quote); Bundesland-Werte nur im interaktiven Dashboard, nicht im statischen HTML. Gegencheck daher über den maschinenlesbaren Datensatz (identische Datenbasis der Seite), s. u.

**Kernaussage 1** ✅ (wörtlich aus Readme.md des Datensatzes, Abschnitt „Indikator ‚Darmkrebs: Sterblichkeit‘“, Zeile 4499; Linktexte entfernt):
> „Zu den wichtigsten beeinflussbaren Risikofaktoren für Darmkrebs gehören Rauchen und Adipositas, gefolgt von Bewegungsmangel, ballaststoffarmer Ernährung, Alkoholkonsum und häufiger Verzehr von rotem beziehungsweise verarbeitetem Fleisch.“

**Kernaussage 2 — Zahlen NRW vs. Bayern** ✅ (TSV am 2026-08-16 frisch von GitHub geladen und unabhängig neu extrahiert — Werte exakt reproduziert; Indikatoren `1020501` Rauchen / `2060201` Adipositas — ⚠️ *die IDs waren in der Vorversion dieser Datei vertauscht*; Berichtsjahr 2019, ab 18 Jahre, Gesamt, altersstandardisiert Europastandard 2013, 95-%-KI):
| Indikator | NRW | Bayern | Deutschland |
|---|---|---|---|
| Rauchen (täglich/gelegentlich) | **31,2 %** (28,9–33,6) | **26,6 %** (24,2–29,1) | 29,6 % |
| Adipositas (BMI ≥ 30) | **19,7 %** (17,9–21,6) | **18,0 %** (15,9–20,2) | 18,8 % |

**Formulierungshinweise (Statistik):**
- Rauchen: 95-%-KIs überlappen kaum → als robusten Unterschied darstellbar.
- Adipositas: KIs überlappen deutlich → nur als „tendenziell höher“ formulieren.
- ⚠️ **Gegenrichtung Alkohol:** „moderates bis hohes Risiko“ in Bayern (37,4 %) höher als NRW (31,4 %) — Alkohol NICHT als NRW-Erklärung verwenden.
- Kontext Bewegung (Ausdauerempfehlung erreicht): NRW 48,5 % vs. Bayern 51,2 % (konsistent, kleiner Unterschied).

**Prüfpunkte Heimmaschine:**
- [x] DOI `10.5281/zenodo.13736662` aufgelöst: Konzept-DOI zeigt auf die jeweils aktuelle Version, derzeit Record 21242132, Version **2026-07-15** (Versions-DOI 10.5281/zenodo.21242132) — Zitat oben entsprechend.
- [x] Zahlen gegengecheckt: TSV frisch geladen, Rauchen 31,2/26,6/29,6 und Adipositas 19,7/18,0/18,8 exakt bestätigt. gbe.rki.de/rauchen liefert Bundesland-Werte nicht im statischen HTML (nur Dashboard) — Datensatz ist die zitierfähige Quelle.
- [x] Optionaler klassischer Journal-Beleg: **bewusst nicht ergänzt** — Quellen-Budget (max. 3–4 neu) ist ausgeschöpft, und der Datensatz ist mit DOI + Version + Lizenz sauber zitierfähig. Falls der Kurs Datensatz-Zitationen ablehnt: JoHM-Artikel zu GEDA 2019/2020-EHIS nachrecherchieren (Kandidat: Journal of Health Monitoring 3/2022, Schienkiewitz et al. zu Übergewicht/Adipositas) — dann eine der anderen Quellen streichen.

**Dient im Bericht:** Ergänzende Erklärung für NRW > Bayern über verhaltensbezogene Risikofaktoren (Rauchen deutlich, Adipositas tendenziell häufiger in NRW).

---

## Quelle 3 (C4): Wirksamkeit von Einladungsverfahren — ERLEDIGT

Drei Kandidaten, alle am 2026-08-16 im Original geöffnet. **Hauptbeleg: 3a (Gruner et al. 2020)** — Deutschland, FIT-basiert (entspricht dem heutigen oKFE-Testverfahren), größte Effektstärke. 3b (Hoffmeister 2017) deckt zusätzlich die Koloskopie-Einladung und den Nullbefund „Brief ohne Test“ ab; 3c (Green 2022) ist die internationale Langzeit-Reserve.

### 3a — Gruner et al. 2020 (Deutschland, RCT, FIT) — HAUPTBELEG

**APA 7:** ✅ (PDF geöffnet, „Cite this as“ S. 423 gegengelesen)
> Gruner, L. F., Hoffmeister, M., Ludwig, L., Meny, S., & Brenner, H. (2020). The effects of differing invitation models on the uptake of immunological fecal occult blood testing—results from a randomized controlled trial. *Deutsches Ärzteblatt International, 117*(25), 423–430. https://doi.org/10.3238/arztebl.2020.0423

**Links (✅ funktionieren, frei zugänglich):**
- DOI: https://doi.org/10.3238/arztebl.2020.0423 → di.aerzteblatt.de/int/archive/article/214403 (HTTP 200, verifiziert 2026-08-16)
- PDF (frei): https://cf.aerzteblatt.de/pdf/di/117/25/m423.pdf
- PubMed: PMID 32885780 · PMC: PMC7490457 (per NCBI-ID-Converter bestätigt)

**Design ✅ (Summary/Methods, S. 423–424):** Dreiarmige RCT des DKFZ (Gruppe Brenner/Hoffmeister) mit der AOK Baden-Württemberg, 17 532 Versicherte im Alter 50–54: (A) Einladungsbrief mit beigelegtem FIT (n = 5850), (B) Einladungsbrief mit niedrigschwelliger FIT-Anforderungsoption (n = 5844), (C) Kontrollgruppe nur Einladungsbrief/Routinepraxis (n = 5838). Registrierung DRKS00011858.

**Effektgrößen ✅ (wörtlich aus Summary → Results, S. 423):**
> „The invitation letter with a FIT enclosed (A) increased usage from 10% to 29.7% compared with the control group (+19.7% points, p < 0.0001; men: +19.4%, women: +18.8%). The invitation letter with a FIT request option (B) increased usage from 10% to 27.7% (+17.7% points, p < 0.0001; men: +17.7%, women: +17.4%).“

> Conclusion, S. 423: „Letters of invitation that include a FIT and those that offer low-threshold access to a FIT achieve strong, comparable increases in the usage of FIT in the context of colorectal cancer screening.“

Detailzahlen: Tabelle 1, S. 425 (Gesamt-FIT-Nutzung binnen 1 Jahr: A 29,7 %, B 27,7 %, C 10,0 %; relative FIT-Nutzung A vs. C 3,0 [95-%-KI 2,7–3,2]).

**Prüfpunkte Heimmaschine (aus Remote-Nachtrag):**
- [x] Original geöffnet (aerzteblatt-PDF), Teilnahmeraten aller drei Arme wörtlich mit Fundstelle gezogen (Summary S. 423; Tabelle 1 S. 425). Remote-Snippet-Werte (29,7 %/27,7 %/~10 %) exakt bestätigt.
- [x] DOI `10.3238/arztebl.2020.0423` aufgelöst (HTTP 200, s. o.).

**Dient im Bericht:** Direktester deutscher RCT-Beleg für die Handlungsempfehlung „Teilnahme steigern“: Persönliche Einladung mit beigelegtem oder leicht anforderbarem Stuhltest verdreifacht die FIT-Nutzung (10 % → ~30 %). FIT-basiert und damit näher am heutigen oKFE-Programm als 3b.

### 3b — Hoffmeister et al. 2017 (Deutschland, SAMS-RCT) — Zusatzbeleg Koloskopie + Nullbefund „Brief ohne Test“

**APA 7:** ✅ (PDF geöffnet, „Cite this as“ S. 87 gegengelesen)
> Hoffmeister, M., Holleczek, B., Zwink, N., Stock, C., Stegmaier, C., & Brenner, H. (2017). Screening for bowel cancer: Increasing participation via personal invitation—a randomized intervention study. *Deutsches Ärzteblatt International, 114*(6), 87–93. https://doi.org/10.3238/arztebl.2017.0087

Deutsche Originalfassung: „Darmkrebsscreening – persönliche Einladung steigert Teilnahmeraten“ (Artikel „Translated from the original German“, S. 92). Studienregistrierung DRKS00006098 (S. 87 u. S. 92). Fundweg: Literaturverzeichnis des Zi-Berichts 20/02 (Referenzen 45/48) — keine Suchmaschine nötig. (helix-PubMed-DB zuerst abgefragt, Endpoint verlangt Auth → Regel „DB vor Websuche“ dokumentiert erfüllt.)

**Links (✅ funktionieren, frei zugänglich):**
- DOI: https://doi.org/10.3238/arztebl.2017.0087 → di.aerzteblatt.de/int/archive/article/186297 (HTTP 200)
- PDF (frei): https://cf.aerzteblatt.de/pdf/di/114/6/m87.pdf
- PubMed: PMID 28266301 · PMC: PMC5341111

**Design ✅ (Summary/Methods, S. 87–88):** SAMS-Studie („Saarland gegen Darmkrebs – Machen Sie mit!“), individuell randomisierte Interventionsstudie im Saarland, 18 560 Personen im Alter 50 (Einladungsbrief + beigelegter gFOBT / Brief ohne Test / keine Einladung) und 16 824 Personen im Alter 55 (Einladung zur Früherkennungskoloskopie / keine Einladung), ab 1. April 2012, Teilnahme via KV-Abrechnungsdaten.

**Effektgrößen ✅ (wörtlich aus Summary → Results, S. 87):**
> „A written invitation to undergo testing of the stool for blood, together with an accompanying test, increased the participation rate within one year by 62% (from 15% to 25%, p <0.001), especially among men (+158% vs. +39% for women).“

> „On the other hand, a written invitation with no accompanying test did not increase the participation rate. A written invitation to undergo colonoscopic screening increased the participation rate within one year by 32% (5.9% vs 4.4%, p <0.001).“

Detailzahlen: Tabelle 1, S. 89 (gFOBT: 25 % Brief+Testkit vs. 15 % Kontrolle; Männer +158 %, Frauen +39 %) und Tabelle 2, S. 90 (Koloskopie: 5,9 % vs. 4,4 %, +32 %; Frauen +36 %, Männer +27 %).

**Einschränkung (ehrlich mitnehmen, S. 92):** Teilnahmeraten bleiben trotz Effekt unter denen organisierter Programme im Ausland; Einladung zum Stuhltest wirkt **nur mit beigelegtem Test**.

**Dient im Bericht:** Ergänzt 3a um zwei Punkte, die Gruner nicht abdeckt: (1) auch die **Koloskopie**-Einladung wirkt (+32 %), (2) ein Brief **ohne** Test wirkt nicht — stützt die konkrete Ausgestaltung der Handlungsempfehlung (Test beilegen, wie in der oKFE-RL diskutiert).

### 3c — Green et al. 2022 (USA, RCT, 9 Jahre) — internationale Langzeit-Reserve

**APA 7:** ✅ (Volltext-XML des PMC-Artikels über GitHub-Mirror geöffnet und gelesen; Verifikation durch Remote-Session)
> Green, B. B., Anderson, M. L., Cook, A. J., Chubak, J., Fuller, S., Meenan, R. T., & Vernon, S. W. (2022). A centralized program with stepped support increases adherence to colorectal cancer screening over 9 years: A randomized trial. *Journal of General Internal Medicine, 37*(5), 1073–1080. https://doi.org/10.1007/s11606-021-06922-2

**Link:** https://pmc.ncbi.nlm.nih.gov/articles/PMC8162159/ (PMCID PMC8162159; gelesenes XML: https://raw.githubusercontent.com/choxos/funded-trials/main/pmc_nih/PMC%208162159.xml)

**Kernaussage 1** ✅ (Abstract, Key Results; UC = usual care):
> "Compared to UC, intervention participants had 21% more covered time over 9 years (57.5% vs. 69.1%; adjusted incidence rate ratio 1.21, 95% confidence interval 1.16–1.25, P < 0.001)."

**Kernaussage 2** ✅ (Abstract, Conclusions):
> "An outreach program that included mailed fecal tests and phone follow-up led to increased adherence to CRC testing and fewer age-eligible individuals without any CRC testing over 9 years."

**Dient im Bericht:** Randomisierter Langzeit-Beleg, dass ein organisiertes Einladungs-/Outreach-Programm (postalische Stuhltests + Erinnerungen) die dauerhafte Screening-Teilnahme signifikant erhöht — Reserve, falls nur eine C4-Quelle Platz hat und internationale Evidenz gewünscht ist.

**Optionale Zusatzthemen (sex differences review, early-onset CRC):** nicht bearbeitet — Quellen-Budget ausgeschöpft, Kernauftrag erfüllt.

---

## Empfehlung zur Übernahme (max. 3–4 neue Quellen) — FINAL

1. **Steffen et al. 2020 (Versorgungsatlas 20/02)** ✅ — regionale Screening-Unterschiede; Teilnahme „weiter ausbaufähig“. Achtung: NRW-KVs liegen nur bei der präventiven Koloskopie leicht unter Bayern, beim KFE-RL-Gesamtmaß gleichauf — vorsichtig formulieren (s. Quelle 1).
2. **RKI-GEDA-Datensatz 2026 (Version 2026-07-15)** ✅ — Risikofaktoren NRW vs. Bayern (Rauchen robust, Adipositas tendenziell).
3. **Gruner et al. 2020 (Dtsch Arztebl Int, RCT)** ✅ — Hauptbeleg Einladungsverfahren: FIT-Nutzung 10 % → 29,7 % durch Einladung mit beigelegtem Test.
4. *Optional:* **Hoffmeister et al. 2017 (SAMS-RCT)** ✅ — ergänzt Koloskopie-Einladung (+32 %) und den Nullbefund „Brief ohne Test“; nur aufnehmen, wenn das Zeichen-Budget es hergibt. Green et al. 2022 bleibt Reserve.

Der Starker-DOI ist kein Neuzugang, sondern Nachtrag zu Teil A (jetzt ✅ mit wörtlichen Fundstellen S. 81/83/84). Damit bleibt das Budget (~8.400 Zeichen Diskussion) eingehalten.
