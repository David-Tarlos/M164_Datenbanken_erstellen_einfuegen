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


# Tag 4 – Datenbanken erstellen und Daten einfügen

Heute habe ich mich intensiv mit der Erstellung und Verwaltung von Fremdschlüsselbeziehungen in relationalen Datenbanken sowie deren Einschränkungen beschäftigt. Dabei lag der Fokus auf der praktischen Umsetzung von **Constraints**, der Implementierung von **Fremdschlüsselbeziehungen** und dem **Forward Engineering** in MySQL/MariaDB.

---

## Was ich heute gelernt habe:

---

### Wiederholung & Vertiefung

- **Recap / Q&A zu Tag 3**: Analyse der Fremdschlüssel-Constraints und deren Anwendung zur Sicherstellung der referenziellen Integrität.
- **Erweiterung des Wissens über Constraints und Fremdschlüsselbeziehungen**: Besonderes Augenmerk auf die Bedeutung von **NOT NULL** und **UNIQUE** für die Wahrung der Datenintegrität.
- **Mengenlehre**: Einführung in Mengenoperationen und deren Anwendung bei **SQL JOINs**.
- **Vorbereitung auf die Anwendung von Forward Engineering**: Praktische Durchführung von SQL-Skripten zur Erstellung der relationalen Datenbankbeziehungen.

---

### Wichtige Konzepte & Umsetzung:

---

#### Beziehungen in relationalen Datenbanken

- **Beziehungen mit Einschränkungen**:
  - **Fremdschlüssel-Constraints** spielen eine entscheidende Rolle beim Aufbau von Beziehungen zwischen Tabellen, um Datenkonsistenz und referenzielle Integrität zu gewährleisten.
  - **NOT NULL (NN)** und **UNIQUE (UQ)** Constraints stellen sicher, dass Fremdschlüsselwerte korrekt und eindeutig sind.
  
- **Beziehungstypen im physischen Modell**:
  - **1:1**: Eine Eins-zu-Eins-Beziehung zwischen zwei Tabellen.
  - **1:m**: Eine Eins-zu-Viele-Beziehung zwischen zwei Tabellen.
  - **m:m**: Eine Viele-zu-Viele-Beziehung, die über eine Transformationstabelle realisiert wird.

---

#### Praktische Umsetzung

- **Erstellung und Implementierung von Beziehungen mit Fremdschlüssel-Constraints**:
  - In MySQL Workbench habe ich Tabellenbeziehungen erstellt und die **Constraints** (NN und UQ) richtig gesetzt, um die Datenintegrität zu sichern.
  - Beispiel für eine **1:m-Beziehung**:
    ```sql
    ALTER TABLE tbl_Ausweis
    ADD CONSTRAINT FK_Ausweis_Fahrer FOREIGN KEY (FahrerID)
    REFERENCES tbl_Fahrer (FahrerID);
    ```

- **Forward Engineering**:
  - Mit **Forward Engineering** habe ich das ERD in SQL-Datenbank-Skripte umgesetzt. Dies ermöglichte es mir, automatisch DDL-SQL-Befehle für die Erstellung von Tabellen und Beziehungen zu generieren.
  - Durch das Erzeugen und Speichern des DDL-SQL-Skripts konnte ich die Tabellenstruktur und die Beziehungen einfach testen.

- **Erweiterung und Testen der Fremdschlüsselbeziehungen**:
  - Das Einfügen von Datensätzen in Tabellen mit existierenden Fremdschlüsselbeziehungen wurde getestet, wobei ich auf die Einhaltung von **referenzieller Integrität** achtete.
  - Dabei überprüfte ich, was passiert, wenn ein **ungültiger Fremdschlüsselwert** eingefügt wird, z.B. ein Wert, der nicht im Primärschlüssel der referenzierten Tabelle existiert.

---

#### Mengenlehre und SQL-Operationen

- **Mengenoperationen und deren Anwendung auf SQL JOINs**:
  - Ich habe mich mit der **Mengenlehre** beschäftigt, die als Grundlage für das Verständnis von SQL-Join-Operationen dient, insbesondere bei der Verknüpfung von Datensätzen aus mehreren Tabellen.
  - Die relevanten **Mengenoperationen** sind **Schnittmenge (∩)**, **Vereinigung (∪)** und **Differenzmenge (\\)**, die bei der Formulierung von SQL-Abfragen und der Verwendung von **JOINs** in komplexeren Abfragen helfen.

- **SELECT JOIN**:
  - **INNER JOIN** und **LEFT JOIN** wurden angewendet, um Daten aus mehreren Tabellen zu kombinieren. Ein praktisches Beispiel:
    ```sql
    SELECT * FROM tbl_Ausweis
    LEFT JOIN tbl_Fahrer
    ON tbl_Ausweis.FahrerID = tbl_Fahrer.FahrerID;
    ```

---

### Fragen, die ich heute beantwortet habe:

- **Wie wird der Fremdschlüssel-Constraint "NOT NULL" erstellt?**
  - Der **NOT NULL**-Constraint wird durch die Definition des Fremdschlüssels mit der Einschränkung auf **NOT NULL** in der Tabelle hinzugefügt, um sicherzustellen, dass der Wert des Fremdschlüssels immer vorhanden ist.

- **Warum wird für jeden Fremdschlüssel ein Index erstellt?**
  - Ein **Index** wird automatisch erstellt, um die **Abfragegeschwindigkeit** zu optimieren. Indizes ermöglichen es, die Fremdschlüsselwerte schneller zu durchsuchen und die referenzielle Integrität effizienter zu überprüfen.

- **Was passiert, wenn ein ungültiger Fremdschlüsselwert eingefügt wird?**
  - Mit einem **Constraint** wird der ungültige Fremdschlüsselwert abgelehnt und verhindert, dass inkonsistente Daten in die Tabelle eingefügt werden.

- **Wie wird der **UNIQUE**-Constraint für Fremdschlüssel im Forward Engineering erstellt?**
  - Der **UNIQUE**-Constraint stellt sicher, dass der Wert des Fremdschlüssels in der Detailtabelle nur einmal vorkommen darf. Dies wird durch die Definition des Fremdschlüssels als **UNIQUE** während des Forward Engineerings erreicht.

---

## Meine Erkenntnisse heute:

- **Beziehungen müssen klar und präzise definiert werden**, insbesondere die **Einschränkungen** für die Fremdschlüsselbeziehungen, um Datenintegrität zu gewährleisten.
- **Fremdschlüssel-Constraints** sind ein essenzielles Werkzeug zur Sicherstellung der referenziellen Integrität in relationalen Datenbanken.
- **Forward Engineering** vereinfacht den Prozess der Datenbankerstellung und hilft, die Struktur schnell und fehlerfrei zu generieren.
- Das Verständnis von **Mengenoperationen** ist entscheidend, um komplexe SQL-Abfragen zu formulieren und Daten korrekt zu verknüpfen.

---

Durch diese Vertiefung der **Beziehungen** und **Constraints** konnte ich ein tieferes Verständnis für die Funktionsweise und die praktischen Anwendungen relationaler Datenbanken entwickeln und die grundlegenden SQL-Befehle sicher anwenden.

# Tag 5 – Datenintegrität, DQL, DCL und SELECT-Abfragen

Heute habe ich mich mit Datenintegrität, Löschoperationen in professionellen Datenbanken und erweiterten SELECT-Abfragen beschäftigt. Der Fokus lag auf den FK-Constraint-Optionen, Aggregatsfunktionen und der Reihenfolge von SELECT-Klauseln.

## Was ich heute gelernt habe:

### 1. Einführung in Datenintegrität und Löschregeln

**Löschen in professionellen DBs:**

- Daten werden selten physisch gelöscht, sondern durch Soft-Deletes markiert (z. B. `is_active = 0` oder Austrittsdatum).
- **Gründe:** Historisierung, Compliance, Vermeidung von Informationsverlust (z. B. in Banken oder Wikis).

**Datenintegrität:**

- 5 Aspekte:  
  - Eindeutigkeit  
  - Referenzielle Integrität  
  - Korrekte Datentypen  
  - Validierung  
  - Beschränkungen (z. B. `CHECK`)
- Unterschied zur Konsistenz:  
  - **Integrität** = Regeln für korrekte Daten  
  - **Konsistenz** = logische Widerspruchsfreiheit

---

### 2. Fremdschlüssel-Constraints (ON DELETE/UPDATE)

**Optionen beim Löschen:**

- `NO ACTION` (Standard): Blockiert Löschen, wenn abhängige Datensätze existieren.
- `CASCADE`: Löscht/aktualisiert abhängige Datensätze automatisch  
  *(Achtung: Risiko von Kettenreaktionen!)*
- `SET NULL`: Setzt Fremdschlüssel auf `NULL`  
  *(nur möglich, wenn Spalte `NULL` erlaubt)*

**Praxisbeispiel:**

```sql
ALTER TABLE tbl_orders  
ADD CONSTRAINT FK_Order_Customer FOREIGN KEY (customer_id)  
REFERENCES tbl_customers(id) ON DELETE CASCADE;
```

# Tag 6 – Subqueries und Bulk-Import mit LOAD DATA INFILE

Heute habe ich mich mit Unterabfragen (Subqueries) und dem massiven Import von Daten via `LOAD DATA INFILE` beschäftigt. Dabei ging es um skalare/nicht-skalare Subqueries sowie die effiziente Überführung von CSV-Daten in MySQL-Tabellen.

---

## Was ich heute gelernt habe:

### 1. Subqueries (Unterabfragen)

**Definition:** Eine Abfrage innerhalb einer anderen Abfrage, um Daten basierend auf Ergebnissen aus anderen Tabellen zu filtern/berechnen.

**Arten:**

- **Skalare Subquery:** Gibt einen einzigen Wert zurück (z. B. `SELECT AVG(price)`).
  - **Operatoren:** `=`, `>`, `<`, etc.
  - **Beispiel:**
    ```sql
    SELECT title FROM books 
    WHERE price > (SELECT AVG(price) FROM books);
    ```

- **Nicht-skalare Subquery:** Gibt mehrere Werte zurück (z. B. Liste mit `IN`).
  - **Operatoren:** `IN`, `NOT IN`, `EXISTS`
  - **Beispiel:**
    ```sql
    SELECT name FROM users 
    WHERE country IN (SELECT country FROM european_countries);
    ```

**Anwendungsorte:** `WHERE`, `FROM`, `HAVING`, `JOIN`

---

### 2. Bulk-Import mit `LOAD DATA INFILE`

**Zweck:** Schnelles Einlesen großer CSV-Dateien in MySQL-Tabellen.

**Wichtige Einstellungen:**

- **Server-Seitig:**
  ```sql
  SET GLOBAL local_infile = 1;  -- Aktiviert Import vom Client
  SHOW VARIABLES LIKE 'secure_file_priv';  -- Sollte leer sein!

  # Tag 7 – Datensicherung und Backup-Strategien

Heute habe ich mich mit Backup-Methoden für Datenbanken und der praktischen Umsetzung von Sicherungen beschäftigt. Dabei ging es um logische/physische Backups, Restore-Prozesse und die Anwendung von Tools wie `mysqldump`.

---

## Was ich heute gelernt habe:

### 1. Backup-Arten und -Strategien

#### 🔁 Voll-Backup (Full Backup)
- **Beschreibung:** Sicherung aller Daten und Strukturen.
- **Vorteil:** Einfache Wiederherstellung (nur eine Datei benötigt).
- **Nachteil:** Hoher Speicherbedarf.

#### 📌 Differentielles Backup
- **Beschreibung:** Sicherung aller Änderungen seit dem letzten Voll-Backup.
- **Vorteil:** Schneller als Voll-Backup, weniger Speicherbedarf.
- **Nachteil:** Redundante Speicherung von Änderungen.

#### 🔄 Inkrementelles Backup
- **Beschreibung:** Nur Änderungen seit dem letzten Backup (egal ob Voll oder Inkrementell).
- **Vorteil:** Geringster Speicherbedarf.
- **Nachteil:** Komplexere Wiederherstellung (alle Backups bis zum Zielzeitpunkt nötig).

#### 💡 Online vs. Offline-Backup
- **Online:** Datenbank bleibt verfügbar (z. B. `mysqldump --single-transaction`).
- **Offline:** Datenbank wird gestoppt (höhere Datenkonsistenz).

---

### 2. Tools für Backups

#### 🛠️ `mysqldump` (logisches Backup)
- **Funktion:** Erzeugt SQL-Skripte mit DDL- und DML-Befehlen.
- **Backup:**
  ```bash
  mysqldump -u root -p --databases tourenplaner > C:/backup/tourenplaner.sql


# Tag 8 – OpenData und erweiterte Datenbankanwendungen

Heute habe ich mich mit OpenData-Quellen beschäftigt und praktische Erfahrungen im Import und der Analyse öffentlicher Datensätze gesammelt. Der Fokus lag auf der Normalisierung von OpenData und der Anwendung von SQL-Abfragen zur Datenanalyse.

---

## Was ich heute gelernt habe

### 1. OpenData: Grundlagen und Quellen

- **Definition:** Öffentlich zugängliche Datensätze von Behörden/Institutionen (z. B. Bundesamt für Statistik, Stadt Zürich)
- **Formate:** CSV, Excel, JSON (häufig mit Metadaten)
- **Anwendungsfälle:** Statistische Analysen, Visualisierungen, Forschungsprojekte

---

### 2. Praktische Übungen mit OpenData

#### a. Steuerdaten der Stadt Zürich

- **Dataset:** Median-Einkommen nach Stadtquartieren (CSV)

**Schritte:**

- **Normalisierung:**
  - Aufteilung in Tabellen für Quartiere, Jahre, Einkommenswerte (`_p25`, `_p50`, `_p75`)
  - Fremdschlüssel für Quartier-ID und Jahr

- **Import:**
  ```sql
  LOAD DATA LOCAL INFILE 'steuerdaten.csv' INTO TABLE einkommen 
  FIELDS TERMINATED BY ',' IGNORE 1 ROWS;




