# Block A – Datenbanken (Access)

## 1. Analyse und ERM auf Grundlage von Prozessen (Datenbanken 1)

### Warum Datenbanken?
- Eine **Datenbank** speichert Daten strukturiert, redundanzarm und widerspruchsfrei; mehrere Nutzer können gleichzeitig zugreifen.
- Abgrenzung zur Tabellenkalkulation (Excel): In Excel entstehen schnell **Redundanzen** (dieselbe Information mehrfach erfasst) und daraus **Anomalien** (Änderungs-, Einfüge-, Löschanomalien). Eine relationale Datenbank vermeidet das durch Aufteilung in verknüpfte Tabellen.

### Grundbegriffe des ERM (Entity-Relationship-Modell)
| Begriff | Bedeutung | Beispiel |
|---|---|---|
| **Entität** (Entity) | Konkretes, unterscheidbares Objekt | „Patientin Meier", „Kurs Statistik I" |
| **Entitätstyp** | Menge gleichartiger Entitäten – wird zur Tabelle | PATIENT, KURS |
| **Attribut** | Eigenschaft eines Entitätstyps – wird zum Tabellenfeld | Name, Geburtsdatum |
| **Schlüsselattribut** | Attribut, das jede Entität eindeutig identifiziert | PatientNr |
| **Beziehung** (Relationship) | Verknüpfung zwischen Entitätstypen | PATIENT *besucht* KURS |
| **Kardinalität** | Wie viele Entitäten dürfen/müssen an der Beziehung teilnehmen | 1:1, 1:n, m:n |

Notation (Chen): Entitätstyp = **Rechteck**, Beziehung = **Raute**, Attribut = **Ellipse/Oval**, Schlüsselattribut unterstrichen.

### Kardinalitäten
- **1:1** – Ein A gehört zu genau einem B und umgekehrt (z. B. Abteilung – Abteilungsleitung). Selten; oft lassen sich beide zu einer Tabelle zusammenfassen.
- **1:n** – Ein A hat mehrere B, jedes B gehört zu genau einem A (z. B. eine Station – viele Patienten). Der Standardfall.
- **m:n** – Viele zu viele (z. B. Patienten – Therapien: ein Patient erhält mehrere Therapien, eine Therapie wird vielen Patienten gegeben). **Muss später über eine Zwischentabelle aufgelöst werden.**

### Vorgehen: Vom Prozess zum ERM
1. **Prozessbeschreibung lesen** und Substantive markieren → Kandidaten für Entitätstypen.
2. **Verben** zwischen den Substantiven markieren → Kandidaten für Beziehungen.
3. Zu jedem Entitätstyp **Attribute** sammeln; ein **Schlüsselattribut** festlegen (im Zweifel künstliche Nummer, z. B. KundenNr).
4. Für jede Beziehung die **Kardinalität** aus dem Prozess ableiten („Ein Kunde kann mehrere Bestellungen aufgeben…" → 1:n).
5. Diagramm zeichnen und gegen die Prozessbeschreibung **gegenprüfen**: Lässt sich jeder Satz des Prozesses im Modell abbilden?

> **Klausurtipp:** Kardinalitäten immer aus beiden Richtungen formulieren („Ein X hat wie viele Y? Ein Y gehört zu wie vielen X?") – das verhindert die häufigsten Fehler.

## 2. ERM nach Access übertragen (Datenbanken 2)

### Umsetzungsregeln ERM → Relationenmodell
1. Jeder **Entitätstyp** wird eine **Tabelle**.
2. Jedes **Attribut** wird ein **Feld** der Tabelle; das Schlüsselattribut wird **Primärschlüssel**.
3. **1:n-Beziehung:** Der Primärschlüssel der 1-Seite wandert als **Fremdschlüssel** in die Tabelle der n-Seite (z. B. StationsNr als Feld in der Patiententabelle).
4. **m:n-Beziehung:** Es wird eine **Zwischentabelle** (Beziehungstabelle) angelegt, die die Primärschlüssel beider Tabellen als Fremdschlüssel enthält (zusammen oft der zusammengesetzte Primärschlüssel). Aus m:n werden damit zwei 1:n-Beziehungen.
5. **1:1-Beziehung:** Entweder Tabellen zusammenlegen oder Fremdschlüssel auf einer Seite.

### Umsetzung in Access
- Tabellen in der **Entwurfsansicht** anlegen, Primärschlüssel setzen (Schlüsselsymbol).
- Menü **Datenbanktools → Beziehungen**: Tabellen hinzufügen, Primärschlüssel per Drag-and-drop auf den passenden Fremdschlüssel ziehen.
- **Referentielle Integrität** aktivieren: Es können keine Datensätze auf der n-Seite angelegt werden, deren Fremdschlüssel auf der 1-Seite nicht existiert; Löschen/Ändern wird kontrolliert (optional mit Aktualisierungs-/Löschweitergabe).

## 3. Access-Grundkonstruktion: Tabellen anlegen (Datenbanken 3)

- **Objekte einer Access-Datenbank:** Tabellen (Datenhaltung), Abfragen (Auswertung), Formulare (Eingabe), Berichte (Ausgabe).
- **Felddatentypen** richtig wählen:
  - *Kurzer Text* (Namen, Telefonnummern – auch Ziffernfolgen, mit denen nicht gerechnet wird!),
  - *Zahl* (Messwerte, Anzahlen), *Währung*, *Datum/Uhrzeit*, *Ja/Nein*, *AutoWert* (automatische laufende Nummer, ideal als Primärschlüssel).
- **Feldeigenschaften:** Feldgröße, Format, Eingabeformat, Gültigkeitsregel (+ Gültigkeitsmeldung), Eingabe erforderlich, Standardwert, Nachschlagefeld (Werteliste oder Bezugstabelle).
- **Ergebnisse checken:** Nach dem Anlegen Testdatensätze erfassen und prüfen, ob Beziehungen und Gültigkeitsregeln greifen (fehlerhafte Eingaben müssen abgewiesen werden, verknüpfte Datensätze müssen sich über die referentielle Integrität korrekt verhalten).

## 4. Formulare und Abfragen (Datenbanken 4)

### Abfragen
- **Auswahlabfrage** (wichtigster Typ): Felder auswählen, Datensätze nach **Kriterien** filtern, sortieren. Die Datenbasis bleibt unverändert – eine Abfrage ist eine gespeicherte Frage, kein Datenduplikat.
- **Kriterien-Syntax:**
  - Vergleiche: `>= 18`, `< #01.01.2020#`, `"Berlin"`
  - Bereiche: `Zwischen 10 Und 20`
  - Muster: `Wie "M*"` (beginnt mit M), Platzhalter `*` und `?`
  - Leere Felder: `Ist Null` / `Ist Nicht Null`
  - **UND** = Kriterien in derselben Zeile, **ODER** = Kriterien in verschiedenen Zeilen (oder Oder-Zeile).
- **Mehrtabellenabfragen** nutzen die definierten Beziehungen (Join über Primär-/Fremdschlüssel).
- **Berechnete Felder:** `Alter: Jahr(Datum())-Jahr([Geburtsdatum])`, Neues Feld mit `Name: Ausdruck`.
- **Funktionen/Gruppierung:** Summe, Mittelwert, Anzahl über die Zeile „Funktion" (Gruppieren nach).
- **Parameterabfrage:** Kriterium in eckigen Klammern `[Bitte Ort eingeben]` → Access fragt den Wert beim Ausführen ab.

### Formulare
- Dienen der komfortablen **Dateneingabe und -anzeige** (eine Maske pro Datensatz statt Tabellenraster).
- Erstellung per **Formular-Assistent** (Tabelle/Abfrage als Datenbasis, Felder auswählen, Layout) und Feinschliff in der **Entwurfs-/Layoutansicht**.
- **Steuerelemente:** Textfelder, Bezeichnungsfelder, Kombinationsfelder (Auswahllisten), Kontrollkästchen, Schaltflächen.
- **Haupt-/Unterformular** bildet 1:n-Beziehungen ab (z. B. Station mit ihren Patienten).

## 5. Export in andere Programme: Excel und SPSS (Datenbanken Ende)

- **Registerkarte „Externe Daten"** in Access: Tabellen oder Abfrageergebnisse exportieren.
- **Export nach Excel:** direkt als .xlsx – Formatierung/Layout bleiben weitgehend erhalten; sinnvoll für Weiterrechnen und Diagramme.
- **Export nach SPSS:** meist über ein Austauschformat (Excel-Datei oder Text-/CSV-Datei), das in SPSS über *Datei → Importieren* eingelesen wird. Dabei beachten:
  - **Erste Zeile = Variablennamen** (kurz, ohne Leer- und Sonderzeichen; keine Umlaute im Variablennamen).
  - **Datentypen prüfen** (Zahl vs. Zeichenfolge, Datumsformat) und in der SPSS-**Variablenansicht** nacharbeiten: Messniveau (nominal/ordinal/metrisch), Wertelabels, fehlende Werte definieren.
  - Codierungen (z. B. 1 = männlich, 2 = weiblich) dokumentieren.
- Merksatz: **Access = Datenhaltung, Excel = Rechnen/Darstellen, SPSS = statistische Auswertung.**

## 6. Datenschutz – DSGVO und das Beispiel SORMAS

### Grundlagen (DSGVO)
- **Personenbezogene Daten:** alle Informationen, die sich auf eine identifizierte oder identifizierbare Person beziehen (Name, Adresse, aber auch IP-Adresse, Patientennummer).
- **Besondere Kategorien** (Art. 9 DSGVO): u. a. **Gesundheitsdaten** – besonders geschützt, Verarbeitung nur mit ausdrücklicher Rechtsgrundlage (z. B. Einwilligung, gesetzliche Pflicht).
- **Grundprinzipien** (Art. 5 DSGVO): Rechtmäßigkeit, Zweckbindung, **Datenminimierung**, Richtigkeit, **Speicherbegrenzung**, Integrität und Vertraulichkeit, Rechenschaftspflicht.
- **Betroffenenrechte:** Auskunft, Berichtigung, Löschung, Einschränkung, Datenübertragbarkeit, Widerspruch.
- Technisch-organisatorische Maßnahmen (TOM): Zugriffsrechte, Verschlüsselung, **Pseudonymisierung/Anonymisierung**, Protokollierung.

### SORMAS als Praxisbeispiel
- **SORMAS** (Surveillance Outbreak Response Management and Analysis System): digitales System der Gesundheitsämter zum **Melde- und Kontaktpersonenmanagement** bei Infektionskrankheiten (bekannt aus der COVID-19-Pandemie).
- Verarbeitet **Gesundheitsdaten** → besondere Kategorie nach Art. 9 DSGVO; Rechtsgrundlage ist das **Infektionsschutzgesetz (IfSG)** mit seinen Meldepflichten – keine Einwilligung nötig, aber strenge Zweckbindung.
- Datenschutz-Aspekte: rollenbasierte Zugriffsrechte (nur zuständiges Gesundheitsamt sieht den Fall), Löschfristen nach Ablauf des Zwecks, Datenweitergabe nur an berechtigte Stellen (z. B. RKI in pseudonymisierter/aggregierter Form).
- Klausurlogik: An SORMAS lässt sich zeigen, **wie eine Fachdatenbank die DSGVO-Prinzipien umsetzt** (Zweckbindung, Datenminimierung, Zugriffskontrolle, Löschkonzept).

## Checkliste Datenbanken

- [ ] Aus einer Prozessbeschreibung Entitäten, Attribute und Beziehungen herausarbeiten
- [ ] Kardinalitäten (1:1, 1:n, m:n) bestimmen und begründen
- [ ] ERM in Chen-Notation zeichnen (Schlüsselattribute unterstreichen)
- [ ] m:n über Zwischentabelle auflösen, Fremdschlüssel richtig platzieren
- [ ] In Access: Tabelle in Entwurfsansicht anlegen, Datentypen und Primärschlüssel setzen
- [ ] Beziehungen mit referentieller Integrität definieren
- [ ] Auswahlabfrage mit UND/ODER-Kriterien, Platzhaltern und berechnetem Feld erstellen
- [ ] Formular mit Assistent erstellen, Zweck von Haupt-/Unterformular erklären
- [ ] Export nach Excel und SPSS durchführen und die Stolpersteine (Variablennamen, Datentypen) nennen
- [ ] DSGVO-Grundprinzipien aufzählen und auf SORMAS/Gesundheitsdaten anwenden
