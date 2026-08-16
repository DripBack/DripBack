# Übergabeprompt Heimmaschine — komplette Literaturrecherche Kolonkarzinom

**Wo liegt alles:**
- Repo: `DripBack/DripBack` (GitHub)
- Branch: `claude/kolonkarzinom-literatur-recherche-8nq28x`
- Draft-PR: https://github.com/DripBack/DripBack/pull/1
- Zwischenstand: `literaturrecherche/QUELLEN_kolonkarzinom_diskussion.md`

```bash
git clone https://github.com/DripBack/DripBack.git
cd DripBack
git checkout claude/kolonkarzinom-literatur-recherche-8nq28x
```

Den folgenden Prompt komplett in die lokale Claude-Code-Session einfügen (Heimmaschine mit Chrome-Anbindung / freiem Internet):

---

## PROMPT (ab hier kopieren)

Du übernimmst die **komplette Literaturrecherche** für das Diskussionskapitel eines Gesundheitsberichts. Eine Remote-Session ohne Internetzugriff hat vorgearbeitet; du führst die Arbeit mit deinem Browser-/Internetzugang zu Ende.

**Arbeitsort:** Repo `DripBack/DripBack`, Branch `claude/kolonkarzinom-literatur-recherche-8nq28x`. Der Zwischenstand liegt in `literaturrecherche/QUELLEN_kolonkarzinom_diskussion.md` — lies diese Datei zuerst vollständig; sie enthält je Angabe ein Verifikationslabel (✅ Dokument geöffnet / 🔶 nur such-verifiziert / ❌ nur Suchsnippet) und offene Checkbox-Prüfpunkte.

### Kontext des Berichts
Gesundheitsbericht über Sterbefälle infolge bösartiger Neubildungen des Kolons (ICD-10 C18–C21), Deutschland vs. NRW vs. Bayern, 2014–2024, Alter 50–95+, nach Geschlecht. Datenbasis: Todesursachenstatistik via gbe-bund.de. Hauptergebnisse: (1) Sterblichkeit sinkt 2014–2024, (2) NRW durchgängig höher als Bayern/Deutschland, (3) Sterblichkeit steigt stark mit dem Alter, (4) Männer > Frauen.

### Lieferformat pro Quelle
Vollständige APA-7-Angabe · frei zugänglicher Link/DOI · 1–2 **wörtlich** belegbare Kernaussagen (mit Fundstelle: Abstract/Seite) · ein Satz, wofür sie im Bericht dient. Keine Fließtexte — nur Quellen + Belege.

### Bereits gesichert (NICHT erneut suchen)
Brenner et al. 2016 (DOI 10.3238/arztebl.2016.0101) · Hoebel et al. 2024 (DOI 10.1007/s00103-024-03862-0) · Starker et al. 2017 (JoHM 2(4):81–87) · Stolpe & Kowall 2025 (DOI 10.1007/s00103-024-03986-3) · Statistisches Bundesamt 2026a/b (Metadaten gbe-bund) · aus dem Teil der Kommilitonin: RKI 2025 Krebs in Deutschland; G-BA 2025 oKFE-RL; Henderson et al. 2021; Czymek et al. 2013; S3-Leitlinie (Langer, 2026); Holzapfel et al. 2020.

### Aufgaben

**1. Verifiziere den Vorarbeits-Stand** (alle `- [ ]`-Prüfpunkte in `QUELLEN_kolonkarzinom_diskussion.md`):
- **Starker et al. 2017:** DOI `10.17886/RKI-GBE-2017-115` über doi.org auflösen; PDF öffnen (https://edoc.rki.de/handle/176904/2904); Autorenliste (laut Vorarbeit: Starker, Buttmann-Schweiger, Kraywinkel, Kuhnert — Korrektur ggü. Übergabe-Brief!) und die Frauen/Männer-Anteile zur Darmspiegelung wörtlich mit Seitenzahl belegen.
- **Steffen et al. 2020, Zi-Versorgungsatlas-Bericht 20/02** (DOI `10.20364/VA-20.02`, PDF: https://www.versorgungsatlas.de/fileadmin/ziva_docs/108/VA_Bericht_20-02_Darmkrebsfr%C3%BCherkennung_2020-05-14.pdf): 1–2 wörtliche Sätze zur regionalen Variation aus der Zusammenfassung (Seitenzahl!), dazu Teilnahmeraten für KV Nordrhein, KV Westfalen-Lippe und KV Bayerns aus Abbildungen/Tabellen. **Ergebnisoffen prüfen**, ob die NRW-Regionen wirklich über Bayern liegen; falls nein, klar vermerken.
- **RKI/GEDA-Zahlen (bereits ✅ aus RKI-GitHub-Datensatz):** Stichprobe: Rauchen NRW 31,2 % / Bayern 26,6 % auf https://www.gbe.rki.de/rauchen gegenchecken. Optional klassischen Journal-Beleg (z. B. JoHM-Artikel zu GEDA 2019/2020-EHIS) ergänzen, falls Datensatz-Zitation im Kurs nicht akzeptiert wird.

**2. Erledige die noch offene Aufgabe C4 — Wirksamkeit von Einladungsverfahren** (Beleg für Handlungsempfehlung „Teilnahme steigern"):
- Suche: deutsch `Einladungsverfahren organisiertes Darmkrebsscreening Teilnahme Wirksamkeit Studie Deutschland oKFE`; englisch `invitation letter colorectal cancer screening participation randomized trial Germany`, `mailed fecal immunochemical test outreach participation`.
- Kandidaten: deutsche RCTs zu Einladungsschreiben ± beigelegtem Stuhltest (DKFZ/Hoffmeister/Brenner-Umfeld), Dtsch Arztebl Int, Cochrane-Review „interventions to increase uptake of colorectal cancer screening".
- Priorität: Deutschland-Bezug > RCT/Review-Qualität > Aktualität. Quelle ÖFFNEN, Effektgröße (Prozentpunkte/OR) wörtlich mit Fundstelle extrahieren, frei zugänglichen Link (PMC/Verlag) angeben.

**3. Optional, nur wenn Zeit übrig:**
- Geschlechterunterschiede biologisch: `sex differences colorectal cancer incidence mortality review`
- Abweichende Befunde/early-onset: `early-onset colorectal cancer incidence trend Germany`

### Regeln
- **Maximal 3–4 neue Quellen insgesamt** (Diskussions-Budget nur ~8.400 Zeichen). Qualität und freie Zugänglichkeit vor Menge.
- Jede Kernaussage muss im **geöffneten Original** wörtlich nachgelesen sein — kein Paraphrasieren aus Suchtreffern. Labels in der Datei erst nach echtem Dokumentabruf auf ✅ hochstufen, Checkboxen abhaken und kurz notieren, was du gesehen hast.
- Hält eine Quelle der Prüfung nicht stand: ersetzen und den Tausch dokumentieren.

### Abschluss
`QUELLEN_kolonkarzinom_diskussion.md` aktualisieren (C4-Abschnitt ausfüllen, Empfehlungsliste finalisieren), committen und auf denselben Branch pushen (aktualisiert automatisch Draft-PR #1). Commit-Message: `Literaturrecherche: Originale verifiziert + Einladungsverfahren ergänzt (Heimmaschine)`. Zum Schluss im Chat eine Tabelle: Quelle · Prüfstatus · Fundstellen — so, dass alles eigenständig gegengeprüft werden kann (Seite, Satz, Suchbegriff).

## PROMPT ENDE
