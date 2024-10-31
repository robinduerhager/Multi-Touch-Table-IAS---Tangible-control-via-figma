Multi-Touch-Table-IAS---Tangible-control-via-figma

Beispielcode, um aus der Figma-Datei mittels des Plugins HTML zu exportieren und Tangible 2 (ID 2) anzusteuern. Bitte öffne die Datei „tangible-2.html“ und kopiere den Code aus dem Body-Bereich in deine Datei.

Schritte:

1. Verknüpfe das Figma-Projekt mit einem HTML-Export-Plugin (z. B. Figma to Code, Anima, TeleportHQ).
2. Erstelle eine lokale Ordnerstruktur mit dem Hauptordner „tangible-control“.
3. Exportiere das Figma-Projekt lokal und lege die HTML-Dateien im Hauptordner „tangible-control“ ab.
4. Exportiere den Ordner "tuio_client_js" vollständig lokal und lege ihn im Verzeichnis „tangible-control“ ab.
5. Integriere den Beispielcode aus „tangible-2.html“ in die HTML-Datei: kopiere den Body-Bereich (ggf. auch den Header-Bereich).
6. Öffne unter Windows (Multi-Touch-Table-IAS) die App „PowerShell“.
7. Wechsle im Terminal zum Ordner auf dem Desktop mit dem Befehl: cd $HOME\Desktop\tangible-control
8. Starte den Python-Interpreter mit dem Befehl: python -m http.server
9. Öffne einen Browser und rufe die Seite auf: localhost:8000/index_241031-2.html
10. Fertig! Der rote Kreis lässt sich nun über Tangible Nr. 2 auf dem Multi-Touch-Table-IAS ansteuern.

Link zum beispielhaften Figma-Projekt (reduzierte Datei mit einfachem roten Kreis)
https://www.figma.com/design/aTJSpxjPOCAhIuuUm7nCv2/Experiment?node-id=0-1&node-type=canvas&t=oFzzWlQFfWQX9R6R-0

Dateien:
- index_241031-1.html    # Erste Version vom 31.10.2024
- index_241031-2.html    # Zweite Version inkl. angepassten <body>-Bereich aus „tangible-2.html“ bei div (roter Kreis wird mittels Tangible-2 auf dem Multi-Touch-Table-IAS angesteuert)
