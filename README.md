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

