# Tag 1 – Meine ersten Schritte mit SQL und Datenbanken

Heute habe ich mit dem Modul 164 begonnen, das sich mit der Erstellung von Datenbanken und dem Einfügen von Daten beschäftigt. Es baut auf dem Modul 162 auf, in dem ich bereits die Grundlagen der Normalisierung und Datenmodellierung kennengelernt habe.

## Was ich heute gelernt habe:

### Einleitung ins Modul:
- Vorstellung der Regeln und Lernziele
- Modulbeschreibung: Implementierung eines relationalen Datenmodells in einem Datenbankmanagementsystem (DBMS)

### Wiederholung von Fachbegriffen aus Modul 162:
- Wichtige Konzepte und Begriffe wurden noch einmal erklärt
- Die Bedeutung der Normalisierung und ihre Schritte (1NF, 2NF, 3NF)

### Grundlagen der Datenmodellierung:
- **Konzeptionelles Datenmodell (ERM):** Abbildung der realen Welt, ohne Berücksichtigung technischer Details
- **Logisches Datenmodell (ERD):** Darstellung der Daten in relationaler Form, inklusive Primär- und Fremdschlüssel
- **Physisches Datenmodell:** Umsetzung des logischen Modells mit konkreten SQL-Befehlen (`CREATE TABLE` usw.)

### Praktische Übungen:

#### Tourenplaner-Aufgabe:
- Analyse einer Busunternehmen-Datenbank
- Zeichnen eines konzeptionellen Modells mit draw.io oder Papier
- Umsetzung des logischen Modells in MySQL Workbench
- Normalisierung bis zur 3. Normalform

### Installation von MySQL (MariaDB) und Workbench:
- Einrichtung einer lokalen Datenbank mit XAMPP
- Erste Tests mit Workbench

## Fragen, die ich heute beantwortet habe:

- **Wozu dient die Normalisierung?** (Vermeidung von Redundanzen, Erhöhung der Konsistenz)
- **Welche drei Modelle gibt es in der Datenmodellierung?** (ERM, ERD, Physisches Modell)
- **Was sind Anomalien in einer Datenbank?** (Einfüge-, Änderungs- und Löschanomalien)

## Meine Erkenntnisse heute:
- Die Datenmodellierung hilft, die Struktur von Daten zu verstehen und effizient zu speichern.
- Die Normalisierung ist ein wichtiger Schritt, um Redundanzen zu vermeiden und eine gute Datenqualität zu gewährleisten.
- Mit MySQL Workbench kann ich Datenbanken visuell modellieren und in SQL umsetzen.

# Tag 2 – Erstellung von Datenbanken und Einfügen von Daten

Heute habe ich mich intensiv mit der Erstellung von Datenbanken und dem Einfügen von Daten in SQL beschäftigt. Dabei konnte ich mein Wissen aus dem vorherigen Modul vertiefen und praktisch anwenden.

## Was ich heute gelernt habe:

### Erstellung einer Datenbank:
- Verwendung von `CREATE DATABASE` zum Anlegen einer neuen Datenbank
- Nutzung von `USE datenbankname;` zur Auswahl der aktiven Datenbank

### Erstellung von Tabellen:
- Definition von Tabellen mit `CREATE TABLE`-Befehl
- Festlegung von Datentypen (`INT`, `VARCHAR`, `DATE` usw.)
- Verwendung von Primärschlüsseln (`PRIMARY KEY`) und Fremdschlüsseln (`FOREIGN KEY`)

### Einfügen von Daten:
- Nutzung von `INSERT INTO` zum Hinzufügen neuer Datensätze
- Einfügen mehrerer Datensätze in einer Anweisung
- Bedeutung der Spaltenreihenfolge und Standardwerte

## Praktische Übungen:

### Kundendatenbank erstellen:
- Erstellen einer Kunden-Tabelle mit Spalten für `KundenID`, `Name`, `Email` und `Geburtsdatum`
- Einfügen von Beispielkunden mit `INSERT INTO`

### Bestellverwaltung:
- Anlegen einer `Bestellungen`-Tabelle mit Verknüpfung zur `Kunden`-Tabelle über einen Fremdschlüssel
- Testen der referentiellen Integrität durch unterschiedliche `INSERT`-Szenarien

## Fragen, die ich heute beantwortet habe:

- **Wie erstelle ich eine relationale Datenbank?** (Durch `CREATE DATABASE` und anschließende Tabellen mit `CREATE TABLE`)
- **Welche Rolle spielen Primär- und Fremdschlüssel?** (Primärschlüssel identifizieren Datensätze eindeutig, Fremdschlüssel stellen Beziehungen zwischen Tabellen her)
- **Wie kann ich Daten effizient in eine Tabelle einfügen?** (Durch `INSERT INTO` und gezielte Nutzung von Default-Werten oder `NULL`)

## Meine Erkenntnisse heute:
- Eine saubere Tabellenstruktur ist essenziell für effiziente Datenverarbeitung.
- Durch das Verwenden von Primär- und Fremdschlüsseln kann die Datenintegrität sichergestellt werden.
- SQL bietet eine flexible Möglichkeit, Daten geordnet und strukturiert einzufügen und zu verwalten.

# Tag 3 – Datenbanken erstellen und Daten einfügen

Heute habe ich mich intensiv mit der Erstellung von Datenbanken und dem Einfügen von Daten in MySQL/MariaDB beschäftigt. Dabei wurden verschiedene Konzepte und Beziehungen innerhalb einer relationalen Datenbank untersucht und praktisch umgesetzt.

## Was ich heute gelernt habe:

### Wiederholung & Vertiefung

- **Recap / Q&A zu Tag 2:** Generalisierung/Spezialisierung, Identifying Relationships in MySQL Workbench
- **Wiederholung der Datentypen aus Modul 162**
- **Erweiterung des Tourenplaners mit neuen Beziehungen**

### Wichtige Konzepte & Umsetzung:

#### Datentypen in MariaDB/MySQL

Ich habe verschiedene Datentypen kennengelernt und in einer Tabelle vervollständigt. Dazu gehören:

- Ganze Zahlen
- Natürliche Zahlen
- Dezimalzahlen (Decimal(M,D))
- Aufzählungstypen
- Boolean (logische Werte)
- Zeichen (einzelnes Zeichen)
- Gleitkommazahlen
- Zeichenketten (feste & variable Länge)
- Datum/Zeit
- Zeitstempel
- Binäre Datenobjekte (z.B. Bilder)
- JSON

#### Beziehungsarten in relationalen Datenbanken

- **Mehrfachbeziehungen:** Eine Entität kann mehrere Beziehungen zu einer anderen Entität haben. Diese Beziehungen müssen eindeutig benannt werden (z. B. unterschiedliche Rollen).
- **Rekursion (strenge Hierarchie):** Eine Entität kann auf sich selbst referenzieren, um eine Hierarchie darzustellen (z. B. Mitarbeiter mit Vorgesetzten).
- **Einfache Hierarchie (mit Zwischentabelle):** Eine Netzwerkstruktur erfordert eine mc:mc-Beziehung mit einer Zwischentabelle.
- **Stücklistenproblem:** Rekursion zur Abbildung von modularen Produkten und deren Bestandteilen.

### Praktische Umsetzung

#### Erweiterung des Tourenplaners

- Einbau der Mehrfachbeziehungen, Rekursion und einfachen Hierarchie
- Umsetzung in MySQL Workbench mit Forward Engineering
- Strukturierung der Datenbasis für spätere Nutzung

#### Datenbearbeitung mit DML-Befehlen (ÜK Modul 106)

- **INSERT:** Einfügen neuer Datensätze in die Tabellen
- **UPDATE:** Aktualisieren vorhandener Datensätze
- **DELETE:** Entfernen von Datensätzen
- **ALTER/DROP:** Strukturänderungen an Tabellen

#### Arbeiten mit SELECT-Befehlen

- **Grundlegende Abfragen:** `SELECT * FROM Tabelle`
- **Filtern mit WHERE:** Einschränkung von Ergebnissen nach bestimmten Kriterien
- **Verknüpfungen (JOINs):** Abrufen von Daten aus mehreren Tabellen
- **Mathematische & logische Funktionen:** Nutzung von `ROUND`, `IF`, `POWER`, `ABS` usw.

#### Hierarchie in der Tourenplaner-Datenbank

- Aufbau einer Unternehmenshierarchie mit einer rekursiven Beziehung
- Beispiel-Mitarbeiterliste mit Zuweisung der Vorgesetzten
- Einfügen und Testen mit SQL-Statements (`UPDATE` mit `SET WHERE IN`)

#### Mehrfachbeziehungen in der Tourenplanung

- Einfügen von Tour-Daten mit Start-, Ziel- und Zwischenorten
- Prüfung der Daten mit `SELECT` und `JOINs`

## Fragen, die ich heute beantwortet habe:

- **Welche Schwierigkeiten gibt es beim Einfügen von Daten mit Fremdschlüssel-Constraints?**
  - Referenzielle Integrität kann verhindern, dass Datensätze eingefügt oder gelöscht werden, wenn abhängige Einträge fehlen.

- **Warum sind NULL-Werte in der Hierarchie-Tabelle problematisch?**
  - In einer Transformationstabelle stellt jede Zeile eine konkrete Beziehung dar, weshalb NULL-Werte vermieden werden müssen.

- **Wann muss eine separate Hierarchie-Tabelle anstelle einer rekursiven Beziehung eingesetzt werden?**
  - Wenn eine Entität mehrere Vorgesetzte haben kann, erfordert dies eine mc:mc-Beziehung mit einer Zwischentabelle.

## Meine Erkenntnisse heute:

- Die Wahl der richtigen Datentypen ist essenziell für die Effizienz und Konsistenz einer Datenbank.
- Beziehungen in einer Datenbank müssen klar definiert und logisch aufgebaut sein.
- SQL bietet mächtige Werkzeuge zur Datenabfrage und -bearbeitung.
- Durch Normalisierung und Strukturierung können Redundanzen und Inkonsistenzen vermieden werden.

