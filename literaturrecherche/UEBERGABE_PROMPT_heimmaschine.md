# Übergabeprompt für die Heimmaschine (Terminal-Variante)

**Wo liegt alles:** GitHub-Repo `DripBack/DripBack`, Branch `claude/kolonkarzinom-literatur-recherche-8nq28x`, Ordner `literaturrecherche/`. Hauptdatei: `QUELLEN_kolonkarzinom_diskussion.md`.

```bash
git clone https://github.com/DripBack/DripBack.git
cd DripBack
git checkout claude/kolonkarzinom-literatur-recherche-8nq28x
```

Den folgenden Prompt komplett in die lokale Claude-Code-Session (mit freiem Internet) einfügen:

---

## PROMPT (ab hier kopieren)

Du arbeitest im Repo `DripBack/DripBack` auf dem Branch `claude/kolonkarzinom-literatur-recherche-8nq28x`. Öffne `literaturrecherche/QUELLEN_kolonkarzinom_diskussion.md`. Die Datei enthält eine Literaturrecherche für einen Gesundheitsbericht über Kolonkarzinom-Sterblichkeit (ICD-10 C18–C21, Deutschland vs. NRW vs. Bayern, 2014–2024).

Die Vorarbeit stammt aus einer Remote-Session **ohne Zugriff auf externe Webseiten** — alle Angaben mit Label 🔶 (nur such-verifiziert) oder ❌ (nur Snippet) müssen jetzt am Original geprüft werden. Deine Aufgabe:

1. **Arbeite alle `- [ ]`-Prüfpunkte in der Datei ab.** Für jeden Prüfpunkt:
   - Öffne/lade die angegebene Original-URL (PDFs herunterladen und lesen, DOIs über doi.org auflösen).
   - Ersetze jeden ❌-Kandidaten durch das **wörtliche Zitat aus dem geöffneten Original** mit exakter Fundstelle (Seitenzahl, Abschnitt) — oder streiche ihn, wenn der Wortlaut nicht belegbar ist. Nichts paraphrasieren, nichts erfinden.
   - Stufe Labels hoch: 🔶/❌ → ✅ nur nach echtem Dokumentabruf. Hake die Checkbox ab (`- [x]`) und notiere dahinter kurz, was du gesehen hast.

2. **Konkret zu prüfen:**
   - **Starker et al. 2017:** DOI `10.17886/RKI-GBE-2017-115` auflösen; Autorenliste und die Frauen/Männer-Anteile (Darmspiegelung letzte 10 Jahre) mit Seitenzahl aus dem PDF (edoc.rki.de/handle/176904/2904) belegen.
   - **Steffen et al. 2020 (Versorgungsatlas 20/02):** PDF öffnen, 1–2 wörtliche Sätze zur regionalen Variation aus der Zusammenfassung ziehen (Seitenzahl!), Teilnahmeraten für KV Nordrhein, KV Westfalen-Lippe und KV Bayerns heraussuchen. **Ergebnisoffen prüfen**, ob die NRW-Regionen wirklich über Bayern liegen — falls nein, das klar vermerken (dann taugt die Quelle nur als Beleg für „regionale Variation generell").
   - **RKI-GEDA-Zahlen (bereits ✅):** Nur Stichprobe — zwei Werte (Rauchen NRW 31,2 %, Bayern 26,6 %) auf https://www.gbe.rki.de/rauchen gegenchecken.
   - **Quelle 3 (Einladungsverfahren):** Falls der Abschnitt in der Datei noch als „folgt" markiert ist oder Prüfpunkte hat, genauso verfahren.

3. **Regeln:** Maximal 3–4 neue Quellen insgesamt übernehmen (Diskussions-Budget ~8.400 Zeichen). Qualität und freie Zugänglichkeit vor Menge. Jede Kernaussage muss im Original nachprüfbar sein. APA 7. Wenn eine Quelle der Prüfung nicht standhält, ersetze sie durch eine bessere und dokumentiere den Tausch.

4. **Abschluss:** Aktualisierte `QUELLEN_kolonkarzinom_diskussion.md` committen und auf denselben Branch pushen. Commit-Message: `Literaturrecherche: Zitate am Original verifiziert (Heimmaschine)`. Zum Schluss eine kurze Tabelle ausgeben: Quelle · Prüfstatus · was geändert wurde.

## PROMPT ENDE
