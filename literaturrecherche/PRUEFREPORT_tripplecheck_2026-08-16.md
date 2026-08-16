# Prüfreport (Triple-Check) — Literaturrecherche Kolonkarzinom-Diskussion

**Datum:** 2026-08-16 · **Branch:** `claude/kolonkarzinom-literatur-recherche-8nq28x` · **Bezugsdatei:** `literaturrecherche/QUELLEN_kolonkarzinom_diskussion.md`

**Prüfmethodik (drei unabhängige Ebenen):**
1. **Dokument-Ebene:** Jedes PDF heruntergeladen und Seite für Seite gerendert gelesen (Erstverifikation).
2. **Zeichen-Ebene:** Text aller vier PDFs per `pdftotext` extrahiert und jedes wörtliche Zitat per exaktem String-Match gegen den extrahierten Text geprüft (Zweitverifikation; Zwei-Spalten-Layouts wurden an den Fundstellen im Kontext gegengelesen). Green 2022 über das PMC-Volltext-XML (114 KB) gegengegrept.
3. **Link-Ebene:** Alle 19 zitierten URLs am 2026-08-16 frisch abgerufen — **19/19 erreichbar** (18× HTTP 200 auf HEAD; gbe.rki.de/rauchen blockt HEAD mit 400, GET liefert 200 mit 322 584 Bytes).

**Befunde des Triple-Checks (beide korrigiert):**
- Hoffmeister-2017-Zitat: Das Original (S. 87) hat einen Druckfehler — nach „p <0.001“ fehlt die schließende Klammer. Die Quellendatei hatte sie stillschweigend ergänzt → jetzt zeichengenau übernommen mit *(sic)*-Vermerk.
- GEDA-Indikator-IDs waren in der Vorversion vertauscht (korrekt: Rauchen = `1020501`, Adipositas = `2060201`) → bereits im Verifikations-Commit korrigiert.

---

## 1 · Starker et al. 2017 — Inanspruchnahme der Darmspiegelung

**APA 7 (gegen Impressum S. 87 „Zitierweise“ geprüft):**
Starker, A., Buttmann-Schweiger, N., Kraywinkel, K., & Kuhnert, R. (2017). Inanspruchnahme der Darmspiegelung in Deutschland. *Journal of Health Monitoring, 2*(4), 81–87. https://doi.org/10.17886/RKI-GBE-2017-115

**Links (Status 2026-08-16):**
| URL | Status |
|---|---|
| https://doi.org/10.17886/RKI-GBE-2017-115 | 200 → löst auf edoc.rki.de/handle/176904/2904 |
| https://edoc.rki.de/handle/176904/2904 | 200 |
| https://edoc.rki.de/bitstream/handle/176904/2904/22s1e1tx0Baw.pdf | 200 (PDF, 7 Seiten, CC BY) |

**Zitate mit Fundstelle (alle per String-Match bestätigt):**
1. **S. 81, Abstract, vorletzter Satz vor „Neue gesetzliche Regelungen…“:**
   „57 % der Frauen und 61 % der Männer im Alter ab 55 Jahren gaben an, dass bei ihnen innerhalb der letzten 10 Jahre eine Darmspiegelung durchgeführt wurde.“
2. **S. 83, rechte Spalte, Abschnitt „Ergebnisse und Einordnung“, 1. Satz:**
   „In Deutschland geben laut GEDA 2014/2015-EHIS-Daten 56,5 % der Frauen und 60,8 % der Männer ab 55 Jahren an, dass bei ihnen innerhalb der letzten 10 Jahre eine Darmspiegelung durchgeführt wurde“ — *Zitat endet vor dem Klammerverweis „(Tabelle 1)“ des Originals.*
3. **S. 83, gleicher Abschnitt, 4. Satz („Im Geschlechtervergleich fällt auf …“):**
   „Im Geschlechtervergleich fällt auf, dass in der Altersgruppe der 70-Jährigen und Älteren der Anteil der Männer, bei denen innerhalb der letzten 10 Jahre eine Darmspiegelung durchgeführt wurde, größer ist als bei den Frauen.“
4. **S. 84, Tabelle 1:** ≥ 70 Jahre: Männer 67,5 % (65,0–70,0), Frauen 59,1 % (56,6–61,6) — Zahlen im extrahierten Text bestätigt.

**Autorenliste (S. 81, linke Randspalte):** Anne Starker, Nina Buttmann-Schweiger, Klaus Kraywinkel, Ronny Kuhnert — alle vier Namen per String-Match bestätigt. Korrektur gegenüber Übergabe-Brief („Starker/Bertz/Saß“ = andere Publikation) bleibt gültig.

---

## 2 · Steffen et al. 2020 — Zi-Versorgungsatlas 20/02

**APA 7 (gegen „Zitierweise“ S. 2 geprüft):**
Steffen, A., Holstiege, J., Hagen, B., Akmatov, M. K., & Bätzing, J. (2020). *Inanspruchnahme der Darmkrebsfrüherkennung in den Jahren 2009 bis 2018: eine Bestandsaufnahme auf Basis bundesweiter vertragsärztlicher Abrechnungsdaten* (Versorgungsatlas-Bericht Nr. 20/02). Zentralinstitut für die kassenärztliche Versorgung in Deutschland (Zi). https://doi.org/10.20364/VA-20.02

**Links (Status 2026-08-16):**
| URL | Status |
|---|---|
| https://doi.org/10.20364/VA-20.02 | 200 → löst auf versorgungsatlas.de …/108/einleitung/ |
| PDF versorgungsatlas.de …/VA_Bericht_20-02_… (26 Seiten, 4,4 MB) | 200 |
| Landing Page …/108/einleitung/ | 200 |

**Zitate mit Fundstelle (alle per String-Match bestätigt):**
1. **S. 1–2, Abstract → „Ergebnisse“, Satzverbund über den Seitenumbruch:**
   „Die Inanspruchnahme der präventiven Koloskopie blieb stabil mit jährlich rund 2,6 % bei Frauen und 2,5 % bei Männern in der primären Zielgruppe der 55- bis 64-Jährigen.“
2. **S. 2, „Ergebnisse“, letzter Satz:**
   „Die regionale Variation in der Inanspruchnahme ist sowohl auf Jahresebene als auch über den 10-Jahres-Zeitraum hoch, doch wird sie teilweise durch den unterschiedlichen Einsatz kurativer Koloskopien abgeschwächt.“
3. **S. 2, „Schlussfolgerung“, 1. Satz:**
   „Die Teilnahme an den Angeboten der darmkrebsbezogenen Früherkennung ist weiter ausbaufähig und variiert deutlich zwischen den Regionen.“
4. **S. 4, Kasten „Kernaussagen“, letzter Punkt:**
   „Die Inanspruchnahme von Angeboten der darmkrebsbezogenen Früherkennung ist von starker regionaler Variation gekennzeichnet.“

**KV-Werte (S. 15, Tabelle 2 — Zeilen wörtlich aus dem extrahierten Text, Spaltenfolge des Originals: Frauen präv. Kolo | präv. Kolo oder ≥3 FOBT | jegliche Kolo | jegliche oder ≥3 FOBT, dann Männer analog):**
```
Bayerns           27,6  45,1  46,8  58,7   27,6  34,5  45,2  49,6
Nordrhein         25,5  44,9  39,5  54,6   25,3  35,6  37,5  45,2
Westfalen-Lippe   24,5  44,7  37,8  53,9   24,4  34,9  36,3  44,5
```
**Prüfergebnis (ergebnisoffen, wie beauftragt):** Präventive Koloskopie: beide NRW-KVs UNTER Bayern (F 25,5/24,5 vs. 27,6; M 25,3/24,4 vs. 27,6). Kombiniertes KFE-RL-Maß: praktisch gleichauf (F 44,9/44,7 vs. 45,1; M 35,6/34,9 vs. 34,5 — hier Nordrhein sogar minimal ÜBER Bayern). In der Quellendatei entsprechend vorsichtig eingeordnet.

---

## 3 · RKI-GEDA-Datensatz (Risikofaktoren NRW vs. Bayern)

**APA 7:**
Robert Koch-Institut. (2026). *Gesundheitsberichterstattung – Daten zu nichtübertragbaren Erkrankungen* (Version 2026-07-15) [Datensatz]. Zenodo. https://doi.org/10.5281/zenodo.13736662

**Links (Status 2026-08-16):**
| URL | Status |
|---|---|
| https://doi.org/10.5281/zenodo.13736662 (Konzept-DOI) | 200 → löst auf Record 21242132 (Version 2026-07-15) |
| https://zenodo.org/records/21242132 | 200 |
| GitHub-Repo robert-koch-institut/…nichtuebertragbaren_Erkrankungen | 200 |
| https://www.gbe.rki.de/rauchen | 200 per GET (HEAD → 400; Bundesland-Werte nur im interaktiven Dashboard, statisches HTML nennt DE-weit 28,9 % rohe Quote 2019) |

**Zahlen (TSV `GBE_Indikatoren_nichtuebertragbarer_Erkrankungen.tsv`, 64 049 Zeilen, am 2026-08-16 frisch geladen und per Skript extrahiert — Filter: Berichtsjahr 2019, Gesamt, Alle Altersgruppen, altersstandardisiert):**
| Kennzahl (Indikator-ID) | NRW | Bayern | Deutschland |
|---|---|---|---|
| Rauchen (`1020501`) | 31,2 % (28,9–33,6) | 26,6 % (24,2–29,1) | 29,6 % |
| Adipositas (`2060201`) | 19,7 % (17,9–21,6) | 18,0 % (15,9–20,2) | 18,8 % |

Werte identisch mit der Vorarbeit der Remote-Session. ⚠️ Korrigiert: Die Indikator-IDs waren dort vertauscht notiert.

**Readme-Zitat (Readme.md des Datensatzes, Abschnitt „Indikator ‚Darmkrebs: Sterblichkeit‘“, Zeile 4499):**
„Zu den wichtigsten beeinflussbaren Risikofaktoren für Darmkrebs gehören Rauchen und Adipositas, gefolgt von Bewegungsmangel, ballaststoffarmer Ernährung, Alkoholkonsum und häufiger Verzehr von rotem beziehungsweise verarbeitetem Fleisch.“

---

## 4 · Gruner et al. 2020 — Einladungsmodelle FIT (C4-Hauptbeleg)

**APA 7 (gegen „Cite this as“ S. 423 geprüft):**
Gruner, L. F., Hoffmeister, M., Ludwig, L., Meny, S., & Brenner, H. (2020). The effects of differing invitation models on the uptake of immunological fecal occult blood testing—results from a randomized controlled trial. *Deutsches Ärzteblatt International, 117*(25), 423–430. https://doi.org/10.3238/arztebl.2020.0423

**Links (Status 2026-08-16):**
| URL | Status |
|---|---|
| https://doi.org/10.3238/arztebl.2020.0423 | 200 → di.aerzteblatt.de/int/archive/article/214403 |
| https://cf.aerzteblatt.de/pdf/di/117/25/m423.pdf | 200 (PDF, frei) |
| https://pmc.ncbi.nlm.nih.gov/articles/PMC7490457/ | 200 (PMCID per NCBI-ID-Converter aus PMID 32885780 bestätigt) |

**Design (S. 423–424 + Figure 1 S. 424):** Dreiarmige RCT, 17 532 AOK-BW-Versicherte 50–54 J.: A Einladung + FIT (n = 5850), B Einladung + FIT-Anforderungsoption (n = 5844), C nur Einladung (n = 5838). Registrierung DRKS00011858 (per String-Match bestätigt).

**Zitate mit Fundstelle (per String-Match bestätigt):**
1. **S. 423, Summary → „Results“, Sätze 1–2:**
   „The invitation letter with a FIT enclosed (A) increased usage from 10% to 29.7% compared with the control group (+19.7% points, p < 0.0001; men: +19.4%, women: +18.8%). The invitation letter with a FIT request option (B) increased usage from 10% to 27.7% (+17.7% points, p < 0.0001; men: +17.7%, women: +17.4%).“
2. **S. 423, Summary → „Conclusion“:**
   „Letters of invitation that include a FIT and those that offer low-threshold access to a FIT achieve strong, comparable increases in the usage of FIT in the context of colorectal cancer screening.“
3. **S. 425, Tabelle 1, Zeile „Total (%)“:** C 583 (10.0) · A 1738 (29.7) · B 1616 (27.7); relative FIT-Nutzung A vs. C 3.0 [2.7; 3.2].

---

## 5 · Hoffmeister et al. 2017 — SAMS-RCT (C4-Zusatzbeleg)

**APA 7 (gegen „Cite this as“ S. 87 geprüft):**
Hoffmeister, M., Holleczek, B., Zwink, N., Stock, C., Stegmaier, C., & Brenner, H. (2017). Screening for bowel cancer: Increasing participation via personal invitation—a randomized intervention study. *Deutsches Ärzteblatt International, 114*(6), 87–93. https://doi.org/10.3238/arztebl.2017.0087

**Links (Status 2026-08-16):**
| URL | Status |
|---|---|
| https://doi.org/10.3238/arztebl.2017.0087 | 200 → di.aerzteblatt.de/int/archive/article/186297 |
| https://cf.aerzteblatt.de/pdf/di/114/6/m87.pdf | 200 (PDF, frei, 10 Seiten) |
| https://pmc.ncbi.nlm.nih.gov/articles/PMC5341111/ | 200 (PMCID per NCBI-ID-Converter aus PMID 28266301) |

**Design (S. 87–88 + Figure 1 S. 88):** SAMS-Studie, individuell randomisiert, Saarland; 18 560 Personen (50 J.): Einladung + gFOBT / Einladung ohne Test / keine Einladung; 16 824 Personen (55 J.): Koloskopie-Einladung / keine Einladung. DRKS00006098 (per String-Match bestätigt).

**Zitate mit Fundstelle (per String-Match bestätigt):**
1. **S. 87, Summary → „Results“, Satz 1:**
   „A written invitation to undergo testing of the stool for blood, together with an accompanying test, increased the participation rate within one year by 62% (from 15% to 25%, p <0.001, especially among men (+158% vs. +39% for women).“ — *(sic: schließende Klammer nach „p <0.001“ fehlt im Original; im Triple-Check entdeckt und in der Quellendatei zeichengenau korrigiert)*
2. **S. 87, Summary → „Results“, Sätze 3–4 (direkt aufeinanderfolgend):**
   „On the other hand, a written invitation with no accompanying test did not increase the participation rate. A written invitation to undergo colonoscopic screening increased the participation rate within one year by 32% (5.9% vs 4.4%, p <0.001).“
3. **Detailzahlen:** Tabelle 1, S. 89 (gFOBT 25 % vs. 15 %; Männer +158 %, Frauen +39 %) · Tabelle 2, S. 90 (Koloskopie 5,9 % vs. 4,4 %, +32 %; Frauen +36 %, Männer +27 %).

---

## 6 · Green et al. 2022 — Langzeit-RCT USA (Reserve)

**APA 7:**
Green, B. B., Anderson, M. L., Cook, A. J., Chubak, J., Fuller, S., Meenan, R. T., & Vernon, S. W. (2022). A centralized program with stepped support increases adherence to colorectal cancer screening over 9 years: A randomized trial. *Journal of General Internal Medicine, 37*(5), 1073–1080. https://doi.org/10.1007/s11606-021-06922-2

**Links (Status 2026-08-16):** DOI 200 · PMC8162159 200 · XML-Mirror (raw.githubusercontent.com/choxos/…) 200.

**Zitate (am 2026-08-16 selbst aus dem XML gegengegrept — nicht mehr nur Remote-Verifikation):**
1. **Abstract → „Key Results“:** "Compared to UC, intervention participants had 21% more covered time over 9 years (57.5% vs. 69.1%; adjusted incidence rate ratio 1.21, 95% confidence interval 1.16–1.25, P < 0.001)."
2. **Abstract → „Conclusions“:** "An outreach program that included mailed fecal tests and phone follow-up led to increased adherence to CRC testing and fewer age-eligible individuals without any CRC testing over 9 years."

---

## 7 · Schlagwort-/Anforderungs-Abdeckung (Auftrag ↔ Quellen)

| Anforderung aus dem Übergabe-Auftrag | Abgedeckt durch | Status |
|---|---|---|
| Starker-DOI auflösen + PDF öffnen | doi.org → edoc.rki.de, PDF gelesen | ✅ |
| Starker-Autorenliste wörtlich belegen | S. 81 (4 Namen per String-Match) | ✅ |
| Frauen/Männer-Anteile Darmspiegelung mit Seitenzahl | S. 81 (57/61 %), S. 83 (56,5/60,8 %) | ✅ |
| Zi 20/02: 1–2 wörtliche Sätze regionale Variation + Seitenzahl | S. 2 (2 Sätze), S. 4 (Kernaussage) | ✅ |
| Teilnahmeraten KV Nordrhein / Westfalen-Lippe / Bayerns | Tabelle 2, S. 15 (8 Werte je KV) | ✅ |
| Ergebnisoffen prüfen ob NRW über Bayern; falls nein vermerken | NEIN bei präv. Koloskopie (NRW unter Bayern), gleichauf beim KFE-RL-Maß — klar vermerkt | ✅ |
| GEDA-Stichprobe Rauchen 31,2/26,6 gegenchecken | TSV frisch extrahiert, exakt bestätigt; gbe.rki.de-Limitierung dokumentiert | ✅ |
| Optional JoHM-Journal-Beleg | Bewusst nicht ergänzt (Budget); Kandidat benannt | ⚪ dokumentiert |
| C4 Einladungsverfahren: Quelle ÖFFNEN, Effektgröße wörtlich, freier Link | Gruner 2020 (Hauptbeleg) + Hoffmeister 2017 (Zusatz), beide PDFs geöffnet, Effektgrößen wörtlich | ✅ |
| Priorität Deutschland > RCT/Review > Aktualität | Beide C4-Belege: deutsche RCTs (DKFZ/Brenner-Umfeld) | ✅ |
| Max. 3–4 neue Quellen | Steffen + GEDA + Gruner (+ optional Hoffmeister) = 3–4 | ✅ |
| Labels erst nach echtem Dokumentabruf auf ✅ | Alle übernommenen Kernaussagen jetzt ✅ | ✅ |
| Optional: sex differences / early-onset CRC | Nicht bearbeitet (Budget), in Datei vermerkt | ⚪ dokumentiert |
| Commit + Push auf denselben Branch (Draft-PR #1) | Commit „Literaturrecherche: Originale verifiziert …“ gepusht | ✅ |

**Gesamtergebnis:** 30 Einzelchecks (Zitate, Zahlen, Autoren, DOIs, Links) — alle bestanden; 2 Korrekturen aus dem Triple-Check (sic-Klammer Hoffmeister, GEDA-ID-Tausch) in der Quellendatei nachgezogen.
