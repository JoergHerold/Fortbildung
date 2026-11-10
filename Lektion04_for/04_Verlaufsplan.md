# Lektion 4: for-Schleife – Verlaufsplan (nur für die Lehrkraft)

Letzte Doppelstunde vor der Kurzarbeit. Am Ende 10 Minuten für die Probe-Kurzarbeit als Hausaufgabe.

**Lernziele** (Plenum, mündlich oder Folie)
- Sie können die Ausgabe einer for-Schleife mit einer Variablentabelle vorhersagen.
- Sie können mit `range` Zahlenfolgen mit Start, Stopp und Schrittweite erzeugen.
- Sie können die Laufvariable im Schleifenkörper verwenden und eine Summe bilden.
- Sie können eine Zählschleife im Struktogramm lesen und in Python umsetzen.

**Drei Schlüsselbegriffe:** Zählschleife (for), range, Laufvariable

## Zeitplan (90 min)

| min | Phase | Sozialform | Hinweis |
|---|---|---|---|
| 5 | Do Now (and/or, Lösung B) | Partnerarbeit | Stoff aus 03b |
| 5 | Lernziele, Schlüsselbegriffe | Plenum | Variablentabelle an Zeile 1 kurz vorführen: neue Methode |
| 10 | Predict mit Variablentabelle | Partnerarbeit | Zeilenzahl ist absichtlich offen (7 Leerzeilen) |
| 5 | Run und Abgleich | Einzelarbeit | typischer Fehler: Zeile „6 s: 90 m“; danach Diagramm-Option kurz vorführen (1 min, siehe unten) |
| 15 | Investigate (5 Fragen) | Partnerarbeit | |
| 10 | Auswertung Investigate | Plenum | Schwerpunkte: Stoppwert und „bis 5“ ↔ `range(1, 6)` (2), Schleifenkörper (5) |
| 15 | Modify (3 Stufen) | Einzelarbeit | gegenüber Raster um 5 min gekürzt; alle Stufen ändern das Starterprogramm: 1 Eingabe der Sekunden, 2 Weg je Sekunde beim Beschleunigen (Formel Weg = Geschwindigkeit · Zeit bleibt, `geschwindigkeit` wächst je Durchlauf um 3; `weg = 3 * sekunde` ist gleichwertig), 3 Summenvariable `gesamt`. Der Text zu 2 nennt den Lösungsweg nicht; mündliche Hilfe: „Wie schnell ist das Fahrzeug in der 2. Sekunde?“, bei der Ausgabe 3, 12, 27: „Wie lange dauert ein Durchlauf?“ |
| 10 | Make Anhalteweg-Tabelle | Einzelarbeit | gegenüber Raster um 5 min gekürzt; Schnelle: Erweiterung, Zusatzaufgabe |
| 5 | Sicherung an einer Schülerlösung | Plenum | Laufvariable, Stoppwert, Schleifenkörper |
| 10 | Probe-Kurzarbeit als Hausaufgabe | Plenum | siehe unten |

Wenn es eng wird: Make in der Stunde nur starten; die Sicherung geht auch am Modify-Programm (steht so im Notebook).

## Diagramm-Option (nur Unterstützung, keine Aufgabe)

- Im Notebook steht oben die Zelle `import diagramm`. Danach zeigt `%%diagramm` als erste Zeile einer Zelle jeden Schleifendurchlauf als Balken; das Programm selbst läuft unverändert.
- Vorführen nach Run: `%%diagramm` über das Starterprogramm setzen, ausführen. Ein Balken entspricht einer Zeile der Variablentabelle. Weitere gute Stellen: fertige Make-Tabelle, Nebel-Zusatzaufgabe.
- Gezeigt wird die Variable, die in der Schleife zuletzt berechnet und mit `print` ausgegeben wird (in Modify 2 `weg`, in Modify 3 `gesamt`). Eine andere Variable wählt man mit ihrem Namen dahinter, zum Beispiel `%%diagramm weg`.
- Es gibt keine Fragen und keine Aufträge zum Diagramm. Alle Aufgaben funktionieren ohne. Nur bei der Zusatzaufgabe steht ein Tipp, das fertige Programm mit `%%diagramm` anzusehen.
- Rückfallebene: Meldet Binder „Cell magic `%%diagramm` not found“ oder „Line magic function `%%diagramm` not found“, die Zelle `import diagramm` erneut ausführen (nötig nach jedem Neustart). Klappt es nicht, die Zeile `%%diagramm` einfach löschen.
- `%%diagramm` darf unter Kommentaren oder Leerzeilen stehen, es muss nicht die erste Zeile der Zelle sein.
- Voraussetzung: `diagramm.py` liegt im selben Ordner wie das Notebook, `matplotlib` steht in der `requirements.txt`.

## Probe-Kurzarbeit besprechen (10 min)

1. Seite 1 kurz durchgehen: Termin (Mittwoch, 25.11.2026), Lerninhalte, Arbeitsweise. Darauf hinweisen: Struktogramme mit Fallauswahl aus Lektion 03b wiederholen.
2. Aufbau zeigen: vier Aufgaben mit steigender Schwierigkeit, wie im Unterricht erst vorhersagen, dann erklären, ändern oder selbst schreiben.
3. Lesehilfe Struktogramme auf Seite 1 vorlesen (Fallauswahl, „von 1 bis 5“ = `range(1, 6)`).
4. Arbeitsauftrag: erst auf Papier ohne Notebook, danach im Notebook `Probe_KA_pruefen.ipynb` selbst prüfen.
5. Musterlösungen erst nach Ablauf der Bearbeitungszeit bereitstellen.

## Dateien

- Schülerinnen und Schüler: `04_for.ipynb`, `diagramm.py`, `img/sg_wegtabelle.png`, `04_for_AB.pdf`, in `Vorbereitung_Inf_1KA`: `Probe_KA_Inf12T.pdf`, `Probe_KA_pruefen.ipynb` mit `img/`
- Lehrkraft: `04_for_Loesung.ipynb`, `04_for_Musterloesung.docx/.pdf`, `Probe_KA_Inf12T_Loesung.docx/.pdf`, `Probe_KA_pruefen_Loesung.ipynb`

Interne BE-Planung der Probe-KA (nicht auf dem Blatt): A1 4 (2+2), A2 5 (2+2+1), A3 6 (2+4), A4 8 (6+2) = 23 BE.
