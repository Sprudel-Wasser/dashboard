# 🌱 Projekt "Bitte stirb nicht" (Plant Monitor)

Willkommen im vermutlich übersichtlichsten GitHub-Repository der Welt. 

Dieses Repo enthält exakt **eine einzige HTML-Datei**. Warum also ein ganzes Repository dafür anlegen? Weil GitHub Pages so freundlich ist, mir diese eine Datei völlig kostenlos als Web-Dashboard zu hosten. 

## 🪴 Worum geht's?
Meine Pflanzen und ich haben ein Kommunikationsproblem. Um zu verhindern, dass sie lautlos vertrocknen, steckt jetzt ein **ESP32-S3** mit kapazitiven Sensoren in der Erde. 

Der Mikrocontroller wacht einmal am Tag aus seinem Deep Sleep auf, funkt die aktuelle Bodenfeuchtigkeit an ThingSpeak und legt sich sofort wieder für 24 Stunden schlafen. Dieses Dashboard holt sich die Daten per API und malt mit Chart.js einen Graphen über die letzten 30 Tage.

## 🚀 Tech Stack (Achtung, hochkomplex)
* **Frontend:** Eine unschuldige `index.html`. Kein React, kein Vue, kein `.env`-Chaos. Einfach pures HTML und Vanilla JavaScript, wie in den guten alten Zeiten.
* **Backend:** ThingSpeak Cloud.
* **Hardware:** Ein ESP32-S3, der 99,9 % seines Lebens verschläft.

## 🛠️ Setup (Falls du das wirklich kopieren willst)
1. Klau dir die `index.html`.
2. Trage oben im Skript deine eigene ThingSpeak `CHANNEL_ID` und den `READ_API_KEY` ein.
3. Lad es bei GitHub Pages hoch. 

*Hinweis: Gegossen werden muss leider immer noch manuell.* 🚰