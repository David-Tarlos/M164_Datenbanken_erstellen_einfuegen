
# 📚 SQL & Datenbanken Lernjournal

## 🌟 Tag 1 – Erste Schritte mit SQL und Datenbanken
📅 **Datum:** 18.02
🎯 **Modul:** 164 (Datenbankerstellung & Dateneinfügung)

### 📖 Heutige Lerninhalte
![bild (4)](https://github.com/user-attachments/assets/7eabf5cd-4d9b-4455-bf50-343d09451d0b)

### 🔍 Vertiefte Themen
- **Datenmodellierung:** ERM → ERD → Physisches Modell
- **Normalisierung:** 1NF, 2NF, 3NF mit Praxisbeispielen
- **Tools:** MySQL Workbench, draw.io

### 💡 Wichtige Erkenntnisse
> Die Normalisierung ist der Schlüssel zur Vermeidung von Redundanzen und sichert Datenqualität.

### ❓ Beantwortete Fragen
| Frage | Antwort |
|-------|---------|
| Wozu dient Normalisierung? | Redundanzvermeidung, Konsistenzsicherung |
| Datenmodell-Arten? | Konzeptionell, Logisch, Physisch |

---

## 🏗️ Tag 2 – Datenbankerstellung & Dateneinfügung
📅 **Datum:** 25.02

### 🛠️ Praktische Übungen
```sql
-- Beispielcode
CREATE TABLE Kunden (
    KundenID INT PRIMARY KEY,
    Name VARCHAR(100),
    Email VARCHAR(100)
);


INSERT INTO Kunden VALUES (1, 'Max Mustermann', 'max@example.com');
```

### 📊 Lernfortschritt
- ✔️ Datenbank erstellen  
- ✔️ Tabellen mit Constraints definieren  
- ✔️ Dateneinfügung mit INSERT  

### 🧩 Wichtige Konzepte
- Primär-/Fremdschlüssel  
- Datentypen (INT, VARCHAR, DATE)  
- Referentielle Integrität  

---

## 🔗 Tag 3 – Datenbankbeziehungen
📅 **Datum:** 04.03

### 🔄 Beziehungstypen
![bild (5)](https://github.com/user-attachments/assets/937ae0a9-4f5a-4bca-bdd0-4f20f12047bb)


### 💡 Erkenntnisse
- Rekursive Beziehungen für Hierarchien  
- Transformationstabellen für m:n-Beziehungen  
- Forward Engineering in MySQL Workbench  

---

## 🛡️ Tag 4 – Datenintegrität & Constraints
📅 **Datum:** 11.03

### 🚦 Constraint-Typen
| Typ | Beschreibung | Beispiel |
|-----|--------------|----------|
| PK  | Primärschlüssel | `id INT PRIMARY KEY` |
| FK  | Fremdschlüssel | `FOREIGN KEY (user_id) REFERENCES users(id)` |
| NN  | NOT NULL | `name VARCHAR(100) NOT NULL` |

### ⚠️ Wichtig
- ON DELETE CASCADE vs. SET NULL  
- UNIQUE Constraints für eindeutige Werte  

---

## 📊 Tag 5 – Datenabfragen (DQL)
📅 **Datum:** 18.03

### 🎯 SELECT-Abfragen
```sql
SELECT 
    c.name AS Kunde,
    COUNT(o.id) AS Bestellungen
FROM 
    customers c
LEFT JOIN 
    orders o ON c.id = o.customer_id
GROUP BY 
    c.name
HAVING 
    COUNT(o.id) > 5;
```

### 🔍 Aggregatfunktionen
- COUNT(), SUM(), AVG()  
- GROUP BY vs. HAVING  

---

## 🔄 Tag 6 – Subqueries & Datenimport
📅 **Datum:** 25.03

### 📥 Bulk-Import
```bash
mysqlimport --local -u root -p db_name data.csv
```

### 📌 Subquery-Typen
- Skalar (ein Wert)  
- Spaltenorientiert (IN, ANY)  
- Tabellenorientiert (FROM-Klausel)  

---

## 💾 Tag 7 – Backups
📅 **Datum:** 01.04

### 🔐 Backup-Strategien
![bild (6)](https://github.com/user-attachments/assets/a203d670-d72d-4d91-94c9-f9fc013c6563)

- ```bash
  # Backup-Code hier einfügen
  ```

### 🛠️ Tools
- mysqldump  
- binäre Backups  
- Point-in-Time-Recovery  

---

## 🌍 Tag 8 – OpenData
📅 **Datum:** 08.04

### 📊 Datenanalyse
- Beispiel: Zürcher Steuerdaten  
- Normalisierung auf 3NF  
- Visualisierung mit Charts  
- JOINs für Quartiervergleiche  

---

## 🎓 Tag 9 – Prüfungsvorbereitung
📅 **Datum:** 15.04

### 📝 Prüfungstipps
- Zeitmanagement  
- SQL-Syntax priorisieren  
- Normalisierungsschritte verinnerlichen  

### 📚 Lernressourcen
- [MySQL Cheat Sheet](#)
- [Normalisierungsbeispiele](#)
- [JOIN Visualizer](#)
