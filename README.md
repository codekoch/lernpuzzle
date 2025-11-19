🧩 <a href=https://codekoch.github.io/lernpuzzle/>.Lernpuzzle - Ein universeller Sortierspiel-Generator</a>

Lernpuzzle ist ein leichtgewichtiges, webbasiertes Tool, mit dem Lehrer, Dozenten und Schüler interaktive Zuordnungsspiele (Matching-Puzzles) erstellen können. Das gesamte Projekt besteht aus einer einzigen HTML-Datei, benötigt keine Installation und keinen Server.

🚀 Schnellstart

Lade die Datei <b>index.html</b> herunter und öffne sie mit einem Browser oder klicke direkt auf diesen Link <b>https://codekoch.github.io/lernpuzzle/</b>.

Verändere das Puzzle nach deinen Wünschen oder lade direkt ein passendes Template (z.B.Template_Java_Basics.json)

Tipp: Du kannst auch KI nutzen, um direkt ein passendes Template für ein anderes Thema zu erstellen (Im Anhang ist ein kleiner Screenshot: https://github.com/codekoch/lernpuzzle/blob/main/Screenshot_Beispiel_KI_Prompt.pdf). 

Klicke auf "Spiel starten", um es selbst zu testen (Hier ein <a href=https://codekoch.github.io/lernpuzzle/Beispiel.html>Beispiel</a> für ein fertiges Puzzle). 

Klicke auf "Gemischtes Spiel herunterladen", um eine neue HTML-Datei zu erhalten, die du weitergeben kannst (Hier ein <a href=https://codekoch.github.io/lernpuzzle/Beispiel_fuerSchueler.html >Beispiel</a>).

✨ Funktionen

Das Projekt ist in zwei Bereiche unterteilt: den Editor (zum Erstellen) und das Spiel (zum Lösen).

Für Ersteller (Editor-Modus)

Keine Installation: Läuft in jedem modernen Browser (Chrome, Firefox, Safari, Edge).

Dynamische Größe: Wähle beliebig viele Zeilen und Spalten für dein Raster.

Rich Content: Die Zellen unterstützen reinen Text, HTML (für Formeln wie H<sub>2</sub>O) und Vektorgrafiken (SVG).

Live-Vorschau: Sieh sofort, wie deine Eingaben als Kachel aussehen werden.

Intelligentes Layout: Automatische Anpassung der Schriftgrößen ("Text-Fitting"), damit Inhalte immer optimal in die Kacheln passen.

Speichern & Laden:

Exportiere Templates (JSON), um den Rohdaten-Status zu sichern.

Lade eine editierbare HTML-Version herunter, um später weiterzuarbeiten.

Verteilung: Generiere mit einem Klick eine fertig gemischte, spielbare HTML-Datei, die du an Schüler verteilen kannst (per E-Mail, Moodle, Teams etc.).

Für Spieler (Spiel-Modus)

Intuitive Bedienung: Drag & Drop Funktionalität (optimiert für Maus und Touch).

iPad & Mobile Ready: Spezielle Optimierungen verhindern unerwünschtes Verhalten auf iOS (z.B. Textauswahl/Suche beim Ziehen) und passen das Layout an kleine Bildschirme an ("Fit-to-Screen").

Feedback-System:

Anzeige der korrekten Zeilen in Echtzeit (z.B. "4 / 8").

Farbliche Markierung: Korrekte Zeilen werden grün umrandet und fixiert.

Zeitmessung: Nach erfolgreichem Lösen wird die benötigte Zeit angezeigt.

Zufallsgenerator: Jedes Mal, wenn die spielbare Datei geöffnet oder "Neu gemischt" wird, ist die Anordnung anders.

Hilfe-Funktion: Ein optionaler Hilfe-Button zeigt Spielregeln oder Hinweise an.

Spielmodi

Es gibt einen speziellen Schalter im Editor: "Korrekte Zeilenreihenfolge erzwingen".

Aus (Standard): Es ist egal, in welcher Zeile eine korrekte Zuordnung liegt. Hauptsache, die Kacheln innerhalb einer Zeile passen zusammen.

An: Die Zeilen müssen exakt an der Position liegen, wie sie im Editor erstellt wurden (gut für Rankings, Abläufe oder feste Strukturen).


🛠 Technische Details

Das Projekt basiert auf reinem HTML5, CSS3 und Vanilla JavaScript.

Single File Application: Der gesamte Code (Logik, Styling, Struktur) befindet sich in einer Datei. Das macht das Teilen extrem einfach.

Datenspeicherung:

Templates werden als .json gespeichert.

Spielbare Dateien enthalten die Daten als JSON-String direkt im Quellcode (const solution = ...).

Responsive Design: Nutzt 100dvh (Dynamic Viewport Height) und Flexbox/Grid, um den Bildschirm auf Mobilgeräten optimal ohne Scrollbalken am Seitenrand zu nutzen.

📂 Template-Format (JSON)

Fortgeschrittene Nutzer können Templates auch direkt als JSON erstellen und importieren:

JSON

{
  "title": "Titel des Spiels",
  "rows": 2,
  "cols": 2,
  "isOrderForced": false,
  "headers": ["Kategorie 1", "Kategorie 2"],
  "solution": [
    ["Inhalt A1", "Inhalt A2"],
    ["Inhalt B1", "Inhalt B2"]
  ],
  "helpText": "Anleitung hier..."
}

🤝 Mitwirken

Beiträge sind willkommen! Wenn du einen Fehler findest oder eine Idee für eine neue Funktion hast, erstelle gerne ein "Issue" oder einen "Pull Request".

📜 Lizenz

Dieses Projekt ist Open Source. Du kannst es frei verwenden, verändern und für Bildungszwecke nutzen.
