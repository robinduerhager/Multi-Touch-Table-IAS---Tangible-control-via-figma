Multi-Touch-Table-IAS---Tangible-control-via-figma

Beispielcode, um aus der Figma-Datei mittels des Plugins Anima HTML, CSS und Bilder zu exportieren und Tangible 2 (ID 2) anzusteuern. Bitte öffne die Datei „tangible-2.html“ und kopiere den Code vonm body-Bereich in deine Datei.

Anleitung:

1. Figma-Projekt mit dem Plugin für HTML-Export (Figma to Code, Anima, TeleportHQ uvm.) verknüpfen.
2. Lokale Ordnerstruktur erstellen: Hauptordner „tangible-control“.
3. Figma-Projekt lokal exportieren: HTML Hauptordner „tangible-control“ ablegen.
5. Ordner "tuio_client_js" muss komplett lokal exportiert werden und in dem Verzeichnis "tangible-control" liegen
6. Beispielcode aus „tangible-2.html“ in HTML integrieren: body-Bereich ggf. auch header-Bereich.
7. Öffne unter Windows (Multi-Touch-Table-IAS) die App "PowerShell"
8. Wechsle zum Ordner auf dem Desktop "cd $HOME\Desktop\tangible-control"
9. Python-Interpreter starten: "python -m http.server"
10. Starte einen Browser und öffne die Seite: "localhost:8000/index_241031-2.html"
11. Fertig: Der rote Kreis lässt sich durch das Tangible Nr. 2 ansteuern!

Link zum beispielhaften Figma-Projekt (reduzierte Datei mit einfachem roten Kreis)
https://www.figma.com/design/aTJSpxjPOCAhIuuUm7nCv2/Experiment?node-id=0-1&node-type=canvas&t=oFzzWlQFfWQX9R6R-0

Dateien:
- index_241031-1.html    # Erste Version vom 31.10.2024
- index_241031-2.html    # Zweite Version inkl. angepassten <body>-Bereich aus „tangible-2.html“ bei div (roter Kreis wird mittels Tangible-2 Multi-Touch-Table-IAS angesteuert)
