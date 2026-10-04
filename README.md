# SVB Platzplan v3 – Staustufenkicker

Mobile PWA für die Platzbelegung und Terminplanung der Fußballabteilung des SV Buckenhofen.

## Gestaltung
- SVB Rot / Weiß / Schwarz
- offizielles Vereinswappen aus der BFV-Medienquelle in der App
- Staustufenkicker-Branding und Vereinsmotto „Sportlich · Vielseitig · Bewährt seit 1946“
- klare Mannschaftsfarben bei einheitlichem SVB-Rahmendesign

## Funktionen
- Wochenplan im 30-Minuten-Raster
- A1/A2 und B1/B2; Spiele/Turniere belegen A oder B komplett
- Herren I, Herren II, AH, U19/A bis U9/F, Bambini/U7, Fußballschule, Verein
- Training, Fußballschule, Liga, Pokal, Freundschaft, Turnier/Kinderfestival, Rasenpflege, Platzsperre, Vereins-/Sondertermin
- Heim/Auswärts, Gegner, Kabinen, Status, Notizen, Bearbeiter und Änderungsgrund
- Serientermine
- Konfliktprüfung
- Monatsübersicht
- Übersicht für Heimspiele, Änderungen, Sperren und Vereinsinfos
- Schnellverschiebung um ±30 Minuten, ±1 Tag und A↔B
- BFV/iCal/ICS-Import
- CSV-Export
- Live-Synchronisierung über Firebase Firestore

## GitHub Pages
Alle Dateien direkt in das Repository `svb-platzplan` hochladen. Danach unter Settings → Pages `Deploy from a branch`, Branch `main`, Ordner `/ (root)` auswählen.

## Firebase
Verwendet das bestehende Projekt `trainingsplatz-sv-buckenhofen`, Firebase Anonymous Authentication und die Collection `events`.

Hinweis: Die aktuelle anonyme Anmeldung ist bewusst eine einfache Pilotlösung. Vor einem breiten öffentlichen Rollout sollte eine echte Trainer-/Admin-Anmeldung ergänzt werden.
