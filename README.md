# Multi-Touch-Table-IAS---Tangible-control-via-figma

Dupliziere dafür die neueste Beispieldatei aus dem Ordner `tangible-control` und integriere den HTML-Code aus dem Figma-Export.

> **Hinweis:** Falls kein Zugang zu einem TUIO-Tisch besteht, kann der Prototyp auch von zuhause aus mit dem [TUIO-Simulator](https://github.com/InteractiveScapeGmbH/tuio-simulator) von Interactive Scape implementiert und getestet werden. Der Simulator steht unter `Releases` zum Download bereit.

## Einstellungen für den TUIO-Simulator
Damit der [TUIO-Simulator](https://github.com/InteractiveScapeGmbH/tuio-simulator) mit den Beispieldateien funktioniert muss dieser wie folgt eingestellt werden:

- **TUIO-Version:** Tuio2  
- **Kommunikationsprotokoll:** WebSocket  
- **Port:** 3343  
- **Servername/Quellname:** Frei wählbar (hat keine erkennbare Auswirkung)  
- **Token-ID:** 2  

Weitere Informationen zur programmatischen Ansteuerung der Tokens findest du in den JavaScript-Dateien im Ordner:  
`./tangible-control/tuio_client_js/src/tuio20/`

## Schritt-für-Schritt Anleitung
1. **Figma-Export-Plugin installieren**  
   Füge deinem Figma-Projekt ein HTML-Export-Plugin hinzu, z. B.:  
   - [Figma to Code (HTML, Tailwind, Flutter, SwiftUI)](https://www.figma.com/community/plugin/842128343887142055/figma-to-code-html-tailwind-flutter-swiftui)  
   - [Anima (React, HTML, CSS, Tailwind, MUI)](https://www.figma.com/community/plugin/857346721138427857/anima-figma-to-code-react-html-css-tailwind-mui-devmode-inspect-react-html-vue-css)  
   - [TeleportHQ (HTML, CSS, React, Vue)](https://www.figma.com/community/plugin/992726161890204477/teleporthq-figma-to-code-export-html-css-react-vue)  

2. **Projekt herunterladen**  
   Lade dieses Projekt beispielsweise über `git clone https://github.com/robinduerhager/Multi-Touch-Table-IAS---Tangible-control-via-figma.git` in einen Ordner deiner Wahl herunter.

3. **Figma-Projekt exportieren**  
   Exportiere dein Figma-Projekt über das Plugin. Lege die exportierten HTML-Dateien in den Ordner `tangible-control`.  
   _Achte darauf, dass die HTML-Dateien im selben Verzeichnis wie der Ordner `tuio_client_js` liegen._

4. **Beispielcode integrieren**  
   Kopiere den `<body>`-Bereich (und falls notwendig den `<head>`-Bereich) der letzten Beispiel-Datei, z. B. `index_241031-3.html`, in den Figma-Export.

5. **Lokalen Server starten**  
   Öffne unter Windows die App **PowerShell**.  
   Wechsle in das Projektverzeichnis per:  
   ```powershell
   cd $HOME\Desktop\Multi-Touch-Table-IAS---Tangible-control-via-figma\tangible-control
   ```
   und starte danach den lokalen Server über das Terminal:
   ```powershell
   python -m http.server
   ```

6. **Projekt im Browser öffnen**  
   Rufe im Browser folgende Adresse auf: [http://localhost:8000/index_241031-3.html](http://localhost:8000/index_241031-3.html)

7. **Testen**  
   Der rote Kreis lässt sich nun über das Tangible mit der ID 2 sowohl auf dem Multi-Touch-Table-IAS als auch im [TUIO-Simulator](https://github.com/InteractiveScapeGmbH/tuio-simulator) ansteuern.

## Beispiel-Figma-Projekt
Hier findest du ein reduziertes Figma-Projekt mit einfachem roten Kreis:
[https://www.figma.com/design/aTJSpxjPOCAhIuuUm7nCv2/Experiment?node-id=0-1&node-type=canvas&t=oFzzWlQFfWQX9R6R-0](https://www.figma.com/design/aTJSpxjPOCAhIuuUm7nCv2/Experiment?node-id=0-1&node-type=canvas&t=oFzzWlQFfWQX9R6R-0)

## Versionen der Beispieldateien
| Datei                 | Beschreibung                                                                                                                                                                                                                             |
| --------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `index_241031-1.html` | Erste Version vom 31.10.2024                                                                                                                                                                                                             |
| `index_241031-2.html` | Zweite Version inkl. angepasstem `<body>`-Bereich aus `tangible-2.html` (Ansteuerung des roten Kreises mit Tangible-ID 2)                                                                                                                |
| `index_241031-3.html` | Dritte Version basierend auf dem offiziellen [Tuio20-Beispiel](https://github.com/InteractiveScapeGmbH/tuio_client_js/blob/main/examples/tuio20.html) von Interactive Scape. Vereinfachte Herangehensweise zur Nutzung des TUIO-Systems. |
