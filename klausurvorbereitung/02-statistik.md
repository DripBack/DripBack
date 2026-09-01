# Block B – Statistik (mit SPSS)

## 1. Definition, Grundbegriffe und Skalenniveaus (Statistik 1)

### Was ist Statistik?
- **Deskriptive Statistik:** beschreibt und verdichtet vorliegende Daten (Tabellen, Kennzahlen, Grafiken).
- **Schließende (Inferenz-)Statistik:** schließt von einer **Stichprobe** auf die **Grundgesamtheit** – mit Wahrscheinlichkeitsaussagen.

### Grundbegriffe
| Begriff | Bedeutung | Beispiel |
|---|---|---|
| Grundgesamtheit | Alle Einheiten, über die eine Aussage getroffen werden soll | alle Pflegekräfte in Deutschland |
| Stichprobe | Untersuchte Teilmenge der Grundgesamtheit | 200 befragte Pflegekräfte |
| Merkmalsträger | Einheit, an der gemessen wird | eine Person |
| Merkmal (Variable) | Untersuchte Eigenschaft | Alter, Geschlecht, Zufriedenheit |
| Ausprägung | Konkreter Wert eines Merkmals | 34 Jahre, „weiblich", „eher zufrieden" |

### Skalenniveaus – das wichtigste Ordnungsprinzip
| Skalenniveau | Eigenschaften | Beispiele | Erlaubt |
|---|---|---|---|
| **Nominal** | nur Kategorien, keine Rangfolge | Geschlecht, Blutgruppe, Diagnose | zählen, Modus |
| **Ordinal** | Rangfolge, aber Abstände nicht interpretierbar | Schulnoten, Zufriedenheit (Likert), Pflegegrad | zusätzlich: Median, Quartile |
| **Metrisch – Intervall** | gleiche Abstände, kein natürlicher Nullpunkt | Temperatur in °C, Jahreszahlen | zusätzlich: Mittelwert, Differenzen |
| **Metrisch – Verhältnis (Ratio)** | natürlicher Nullpunkt | Alter, Gewicht, Einkommen | zusätzlich: Verhältnisse („doppelt so viel") |

- Das Skalenniveau entscheidet, **welche Kennzahlen, Grafiken und Tests zulässig** sind – klassische Klausurfrage!
- In SPSS wird das Messniveau in der **Variablenansicht** hinterlegt (nominal / ordinal / metrisch „Skala").
- Außerdem: **diskrete** Merkmale (abzählbare Werte, z. B. Kinderzahl) vs. **stetige** Merkmale (jeder Zwischenwert möglich, z. B. Körpergröße).

## 2. Häufigkeiten, Lage- und Streuungsmaße (Statistik 2)

### Häufigkeiten
- **Absolute Häufigkeit** n_i: Anzahl der Fälle einer Ausprägung.
- **Relative Häufigkeit** f_i = n_i / n (Anteil, oft in %).
- **Kumulierte Häufigkeit:** aufsummiert bis zur jeweiligen Ausprägung – nur sinnvoll ab **Ordinalskala**.
- SPSS: *Analysieren → Deskriptive Statistiken → Häufigkeiten*.

### Lagemaße
| Maß | Berechnung/Idee | Ab welchem Skalenniveau |
|---|---|---|
| **Modus** (Modalwert) | häufigste Ausprägung | nominal |
| **Median** | Wert in der Mitte der geordneten Reihe (50 %-Punkt) | ordinal |
| **Arithmetisches Mittel** | Summe aller Werte / n | metrisch |
| **Quartile** | Q1 = 25 %, Q2 = Median, Q3 = 75 % | ordinal |

- Der **Median ist robust** gegen Ausreißer, der Mittelwert nicht (Beispiel Einkommen!).
- Bei schiefen Verteilungen weichen Mittelwert und Median auseinander: rechtsschief → Mittelwert > Median.

### Streuungsmaße
| Maß | Idee | Skalenniveau |
|---|---|---|
| **Spannweite** (Range) | Maximum − Minimum | metrisch (grob) |
| **Interquartilsabstand** (IQR) | Q3 − Q1, die „mittleren 50 %" | ordinal/metrisch |
| **Varianz** s² | mittlere quadrierte Abweichung vom Mittelwert | metrisch |
| **Standardabweichung** s | Wurzel aus der Varianz – gleiche Einheit wie die Daten | metrisch |

- Interpretation: Große Standardabweichung = Werte streuen weit um den Mittelwert.
- Stichprobenvarianz: Division durch **n − 1** (so rechnet auch SPSS).

## 3. Grafische Darstellungen und univariate deskriptive Analysen (Statistik 3)

### Welche Grafik für welches Merkmal?
| Grafik | Geeignet für | Hinweis |
|---|---|---|
| **Balken-/Säulendiagramm** | nominal, ordinal | Kategorien mit Lücken zwischen den Balken |
| **Kreisdiagramm** | nominal (wenige Kategorien) | zeigt Anteile am Ganzen |
| **Histogramm** | metrisch (klassiert) | Säulen ohne Lücken; zeigt Verteilungsform |
| **Boxplot** | ordinal/metrisch | Median, Quartile, Whisker, Ausreißer auf einen Blick |
| **Liniendiagramm** | Verläufe über die Zeit | |

### Univariate Analyse = eine Variable beschreiben
- **Nicht grafisch:** Häufigkeitstabelle + passende Lage- und Streuungsmaße (je nach Skalenniveau).
- **Grafisch:** passende Grafik (siehe Tabelle) + Beschreibung der **Verteilungsform**: symmetrisch vs. schief (links-/rechtsschief), ein- vs. mehrgipflig, Ausreißer.
- **Boxplot lesen können:** Box = IQR (Q1 bis Q3), Linie in der Box = Median, Whisker = Bereich ohne Ausreißer, Punkte/Sterne = Ausreißer/Extremwerte.
- SPSS: *Häufigkeiten* (mit Diagrammen), *Deskriptive Statistik*, *Explorative Datenanalyse* (liefert Boxplots), *Diagramme → Diagrammerstellung*.

## 4. Bivariate deskriptive Analysen und Korrelation (Statistik 4)

### Zwei Variablen gemeinsam betrachten
- **Nominal/ordinal × nominal/ordinal:** **Kreuztabelle** (Kontingenztafel) mit Zeilen-/Spaltenprozenten; grafisch: gruppierte oder gestapelte Balken.
- **Metrisch × metrisch:** **Streudiagramm** (Scatterplot) – Richtung, Form und Stärke des Zusammenhangs beurteilen.
- **Metrisch × nominal:** Gruppenvergleich mit Mittelwerten/Boxplots je Gruppe.

### Korrelation
- **Pearson-Korrelationskoeffizient r:** misst den **linearen** Zusammenhang zweier **metrischer** Variablen. Wertebereich **−1 bis +1**.
  - r > 0: positiver Zusammenhang (je mehr X, desto mehr Y), r < 0: negativ, r ≈ 0: kein linearer Zusammenhang.
  - Faustregeln zur Stärke: |r| ≈ 0,1 schwach, ≈ 0,3 mittel, ≥ 0,5 stark (kursabhängig – im Skript nachsehen).
- **Spearman-Rangkorrelation ρ (rho):** für **ordinale** Daten oder metrische Daten mit Ausreißern/nicht-linearem, aber monotonem Zusammenhang.
- **Korrelation ≠ Kausalität!** Ein Zusammenhang beweist keine Ursache-Wirkung (Scheinkorrelation, Drittvariablen – Beispiel: Eisverkauf und Sonnenbrände korrelieren wegen des Wetters).
- SPSS: *Analysieren → Korrelation → Bivariat* (Pearson/Spearman ankreuzbar); Kreuztabellen unter *Deskriptive Statistiken → Kreuztabellen*.

## 5. Einführung in die schließende Statistik (Statistik 5)

- Ziel: von der **Stichprobe auf die Grundgesamtheit** schließen; da die Stichprobe zufällig ist, sind Aussagen nur mit **Wahrscheinlichkeit** möglich.
- **Normalverteilung:** symmetrische Glockenkurve; viele Merkmale und v. a. **Stichprobenmittelwerte** (zentraler Grenzwertsatz) sind annähernd normalverteilt. Merkregel: ca. 68 % der Werte innerhalb ±1s, ca. 95 % innerhalb ±2s um den Mittelwert.
- **Standardfehler:** Streuung des Stichprobenmittelwerts (s/√n) – je größer die Stichprobe, desto genauer die Schätzung.
- **Schätzen:**
  - **Punktschätzung:** ein Wert (z. B. Stichprobenmittelwert als Schätzer für den Populationsmittelwert).
  - **Intervallschätzung / Konfidenzintervall:** Bereich, der den wahren Wert mit z. B. 95 % Vertrauenswahrscheinlichkeit überdeckt.
- **Testen – die Logik des Hypothesentests:**
  1. **H0 (Nullhypothese):** kein Unterschied / kein Zusammenhang. **H1 (Alternativhypothese):** es gibt einen Unterschied/Zusammenhang.
  2. **Signifikanzniveau α** festlegen (üblich 0,05 = 5 %).
  3. Test rechnen → **p-Wert**: Wahrscheinlichkeit, ein mindestens so extremes Ergebnis zu erhalten, **wenn H0 gilt**.
  4. Entscheidung: **p ≤ α → H0 verwerfen** („signifikant"); p > α → H0 beibehalten (nicht „bewiesen"!).
- **Fehlerarten:** **Fehler 1. Art (α):** H0 fälschlich verworfen. **Fehler 2. Art (β):** H0 fälschlich beibehalten.

## 6. Schätzen und Testen I: t-Verteilung und t-Test (Statistik 6)

### t-Verteilung
- Ähnelt der Normalverteilung, hat aber **breitere Ränder**; Form hängt von den **Freiheitsgraden (df)** ab. Mit wachsendem n nähert sie sich der Normalverteilung an.
- Wird verwendet, wenn die Standardabweichung der Grundgesamtheit unbekannt ist (Normalfall) und aus der Stichprobe geschätzt wird.

### Die drei t-Tests
| Test | Fragestellung | Beispiel |
|---|---|---|
| **Einstichproben-t-Test** | Weicht der Mittelwert von einem vorgegebenen Wert ab? | Ist der mittlere BMI der Stichprobe ≠ 25? |
| **t-Test für unabhängige Stichproben** | Unterscheiden sich zwei **verschiedene** Gruppen im Mittelwert? | Frauen vs. Männer: Zufriedenheit |
| **t-Test für verbundene (gepaarte) Stichproben** | Unterscheiden sich zwei Messungen **derselben** Personen? | vorher vs. nachher einer Intervention |

- **Voraussetzungen:** metrisch skalierte Testvariable, (annähernd) Normalverteilung (bei großen Stichproben unkritisch), bei unabhängigen Stichproben: Varianzhomogenität → SPSS prüft das mit dem **Levene-Test** (Levene p > 0,05 → Zeile „Varianzen sind gleich" lesen, sonst die korrigierte Zeile).
- **SPSS:** *Analysieren → Mittelwerte vergleichen → t-Test bei (un)abhängigen Stichproben / bei einer Stichprobe*.
- **Interpretation in der Klausur (Schema):**
  1. Hypothesen formulieren (H0: μ1 = μ2).
  2. Signifikanz (2-seitig) im Output ablesen.
  3. p ≤ 0,05 → signifikanter Unterschied, H0 verwerfen; p > 0,05 → kein signifikanter Unterschied.
  4. Ergebnis inhaltlich formulieren („Die Gruppen unterscheiden sich signifikant im mittleren …, t(df) = …, p = …").

## 7. Schätzen und Testen II: Chi-Quadrat-Test (Statistik 7)

- **Einsatz:** Zusammenhang zweier **nominaler** (oder ordinaler) Variablen – Auswertung einer **Kreuztabelle**. („Hängt Rauchen vom Geschlecht ab?")
- **Idee:** Vergleich der **beobachteten** Häufigkeiten mit den **erwarteten** Häufigkeiten, die bei Unabhängigkeit gelten würden. Erwartete Häufigkeit pro Zelle = (Zeilensumme × Spaltensumme) / Gesamtzahl.
- Je größer die Abweichung, desto größer χ²; mit **Freiheitsgraden df = (Zeilen − 1) × (Spalten − 1)** wird der p-Wert bestimmt.
- **Hypothesen:** H0: Die Variablen sind unabhängig (kein Zusammenhang). H1: Es besteht ein Zusammenhang.
- **Voraussetzung:** erwartete Häufigkeiten ausreichend groß – Faustregel: **alle (bzw. mind. 80 % der) erwarteten Häufigkeiten ≥ 5** (SPSS gibt eine Fußnote aus; sonst exakter Test nach Fisher).
- Der Chi-Quadrat-Test sagt nur, **dass** es einen Zusammenhang gibt – die **Stärke** liefern Zusammenhangsmaße wie **Cramérs V** (0 bis 1) bzw. Phi.
- **SPSS:** *Deskriptive Statistiken → Kreuztabellen → Schaltfläche „Statistiken" → Chi-Quadrat* (+ Phi/Cramérs V); unter „Zellen" erwartete Häufigkeiten und Prozente anfordern.
- **Interpretation:** „Asymptotische Signifikanz" der Zeile **Chi-Quadrat nach Pearson** ablesen → p ≤ 0,05: signifikanter Zusammenhang, H0 verwerfen; Richtung/Muster anhand der Zeilen-/Spaltenprozente beschreiben.

## Übersicht: Welcher Test / welche Kennzahl wann?

| Situation | Skalenniveau | Verfahren |
|---|---|---|
| Eine Variable beschreiben | nominal | Häufigkeiten, Modus, Balken-/Kreisdiagramm |
| Eine Variable beschreiben | ordinal | + Median, Quartile, kumulierte %, Boxplot |
| Eine Variable beschreiben | metrisch | + Mittelwert, s, Histogramm |
| Zusammenhang | nominal × nominal | Kreuztabelle, **Chi-Quadrat**, Cramérs V |
| Zusammenhang | ordinal × ordinal | **Spearman-Rangkorrelation** |
| Zusammenhang | metrisch × metrisch | Streudiagramm, **Pearson-Korrelation** |
| Mittelwert vs. fester Wert | metrisch | **Einstichproben-t-Test** |
| 2 unabhängige Gruppen | metrisch (+ Gruppierungsvariable) | **t-Test unabhängige Stichproben** |
| 2 Messungen derselben Personen | metrisch | **t-Test verbundene Stichproben** |

## Checkliste Statistik

- [ ] Grundgesamtheit, Stichprobe, Merkmal, Ausprägung sicher definieren
- [ ] Skalenniveau beliebiger Beispielvariablen bestimmen und begründen
- [ ] Zu jedem Skalenniveau die zulässigen Lage-/Streuungsmaße nennen
- [ ] Häufigkeitstabelle (absolut, relativ, kumuliert) berechnen und interpretieren
- [ ] Median vs. Mittelwert: Robustheit und Schiefe erklären
- [ ] Passende Grafik je Skalenniveau wählen; Boxplot und Histogramm lesen
- [ ] Kreuztabelle mit Zeilen-/Spaltenprozenten interpretieren
- [ ] Pearson vs. Spearman abgrenzen; r interpretieren; „Korrelation ≠ Kausalität" erklären
- [ ] Logik des Hypothesentests (H0/H1, α, p-Wert, Fehlerarten) erklären
- [ ] Konfidenzintervall interpretieren
- [ ] Die drei t-Tests unterscheiden und SPSS-Output (inkl. Levene-Test) interpretieren
- [ ] Chi-Quadrat-Test: erwartete Häufigkeiten, df, Voraussetzung ≥ 5, Cramérs V, Output interpretieren
