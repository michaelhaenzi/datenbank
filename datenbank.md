Datenbank
---------

###Was ist eine Datenbank?

* Alle wichtigen Informationen werden in einer Datenbank abgelegt
* Es ist elektronisches Verwaltungssystem

###Woraus besteht eine Datenbank?

Eine Datenbank(-system/ DBS) besteht aus zwei Teilen:

1. Bereitgestellte Informationen werden in Datensätzen (Records) gebündelt und in der Datenbank hinterlegt
2. Software zur Verwaltung der Datenbank, Datenbankmanagementsystem (DBMS)

![DBS](dbs.PNG)

###DBMS - Was ist das?

Es werden die Grundlagen der Datenbank festgelegt. Die Grundlage für eine Datenbank ist das Datenbankmodell. Das DBMS ist zuständig für die:

* Sicherheit
* Transaktion
* Integrität
* Anfrageoptimierung
* Anwendungsunterstützung
* Sprachen
* DML, DDL, DCL
* Mehrbenutzerfähigkeit
* Konsistenz
* Backup

###Datenbankmodell

Es werden die Grundlagen der Datenbank festgelegt. Die Grundlage für eine Datenbank ist das Datenbankmodell. Das DBMS ist zuständig für die:

* Generische Datenstruktur
* Generische Operatoren
* Integritätsbedingungen

Das weitverbreitetste Datenbankmodell ist das relationale Datenbankmodell.

###Relationales Datenbankmodell

Sie stellt eine mathematische Beschreibung einer Tabelle und ihre Beziehung zu anderen möglichen Tabellen dar. Des Weiteren ist die relationale Algebra auch die Grundlage für die Datenbanksprache SQL. Relationale Datenbankmodelle sind vergleichsweise mit anderen Modellen sehr einfach und flexibel zu erstellen und zu steuern. <br><br>
Die Datenbank kann man sich unter einer Sammlung von Tabellen und Beziehungen vorstellen, die miteinander verknüpft sind. Jede Zeile (auch Tupel genannt) in einer Tabelle ist ein Datensatz (record). Jedes Tupel besteht aus einer großen Reihe von Attributen (Eigenschaften), den Spalten der Tabelle. Ein Relationsschema legt dabei die Anzahl und den Typ der Attribute für eine Tabelle fest.

![relationale DB](relationaledb.PNG)

Des Weiteren können Verknüpfungen (Beziehungen) über sogenannte Primärschlüssel hergestellt werden, um bestimme Attribute, die den gleichen Primärschlüssel oder in einer Detailtabelle als Fremdschlüssel besitzen, abzufragen.

###SQL-Befehle

| SQL-Befehl | Syntax | Beschreibung |
| :----------: | ------ | ------------ |
| `SELECT`     | `SELECT Spaltenname FROM Tabellenname` |  |
| `DISTINCT` | `SELECT DISTINCT Spaltenname FROM Tabellenname` |  |
| `WHERE` | `SELECT Spaltenname FROM Tabellenname WHERE Spaltenname = Wert` |  |
| `AND` | `SELECT Spaltenname FROM Tabellenname WHERE Spaltenname1 = Wert1 AND Spaltenname2 = Wert2` |  |
| `OR` | `SELECT Spaltenname FROM Tabellenname WHERE Spaltenname1 = Wert1 OR Spaltenname2 = Wert2` |  |
| `IN` | `SELECT Spaltenname FROM Tabellenname WHERE Spaltenname IN ('Wert1', 'Wert2')` |  |
| `BETWEEN` | `SELECT Spaltenname FROM Tabellenname WHERE Spaltenname BETWEEN 'DATUM1' AND 'DATUM2'` |  |
| `LIKE` | `SELECT Spaltenname FROM Tabellenname WHERE Spaltenname LIKE 'MUSTER'` |  |
| `ORDER BY` | `SELECT Spaltenname FROM Tabellenname WHERE Spaltenname LIKE 'MUSTER'` |  |
| `GROUP BY` | `SELECT spaltenname FROM tabellenname [WHERE Bedingung] GROUP BY spaltenname` |  |
| `HAVING` | `SELECT spaltenname FROM tabellenname [WHERE Bedingung] GROUP BY spaltenname HAVING Ausdruck;` |  |

###Weitere SQL-Befehl Funktionen

**WHERE-Befehl**
* Gleich (=) oder Ungleich (<>)
* Grösser als (>) oder Kleiner als (<)
* Grösser gleich (>=) oder Kleiner gleich (<=)

**LIKE-Befehl:**
* `_` :point_right: Ein beliebiges Zeichen
* `%` :point_right: Eine beliebige Zeichenkette

**ORDER BY-Befehl**
* `ASC` :point_right: Das Ergebnis wird aufsteigend sortiert
* `DESC` :point_right: Das Ergebnis wird absteigend sortiert

**GROUP BY-/ HAVING-Befehl**
* `AVG()` :point_right: Durchschnittswert (Mittelwert)
* `COUNT()` :point_right: Anzahl
* `MAX()` :point_right: MAX (Höchster Wert)
* `MIN()` :point_right: MIN (Kleinster Wert)
* `SUM()` :point_right: SUMME
* `FIRST()` :point_right: Erster Wert der Spalte
* `LAST()` :point_right: Letzter Wert der Spalte
* `UCASE()` :point_right: Konvertiert in Grossbuchstaben
* `LCASE()` :point_right: Konvertiert in Kleinbuchstaben
* `MID()` :point_right: Extrahiert Buchstabenreihe
* `LEN()` :point_right: Zeichenlänge des Wertes
* `ROUND()` :point_right: Runden (VRUNDEN)
* `NOW()` :point_right: Aktuelles Datum und Uhrzeit
* `FORMAT()` :point_right: formatiert nach gewünschtem Format
