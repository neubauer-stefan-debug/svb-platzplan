# SVB Platzplan v7

Mobile PWA für die Platz- und Terminplanung der Fußballabteilung des SV Buckenhofen.

## Neu in v7 – BFV-Vereinsspielplan als PDF
- Im Adminbereich kann die offizielle **BFV-Vereinsspielplan-PDF** für den gesamten SV Buckenhofen hochgeladen werden.
- Die App liest die PDF direkt im Browser mit PDF.js aus; die Datei wird nicht an einen zusätzlichen Server geschickt.
- Es werden automatisch **nur erkannte Heimspiele des SV Buckenhofen** in eine Prüfliste übernommen.
- Mannschaft, Wettbewerb/Terminart und Gegner werden soweit möglich automatisch erkannt.
- Vor dem Import können Mannschaft, Gegner, Platz A/B und Spieldauer korrigiert werden.
- Heimspiele werden optisch deutlich als **HEIMSPIEL** markiert.
- Standardmäßig werden **2 Kabinen – Heim + Gast** reserviert.
- Der Platz wird automatisch **30 Minuten vor Anstoß bis 30 Minuten nach dem errechneten Spielende** blockiert.
- Die eigentliche Anstoßzeit und das Spielende bleiben separat am Termin gespeichert und sichtbar.
- Standard-Spieldauern: Herren/A 90, B 80, C 70, D 60, E 50 Minuten; Kinderfestival/Turnier 120 Minuten. In der Prüfliste kann die Dauer angepasst werden.
- Duplikate aus wiederholten BFV-Imports werden anhand Quelle/Datum/Anstoß/Mannschaft/Gegner übersprungen.
- Bei BFV-Spielstätte Platz 1/2 kann optional automatisch A/B vorgeschlagen werden; ansonsten gilt der gewählte Standardplatz.

## Aus v6 weiterhin enthalten
- Trainer-Auswahl + 4-stellige PIN ohne Google/E-Mail.
- Rollen Trainer / Vollzugriff / Admin.
- A1/A2, B1/B2, C-Platz; Spiele reservieren A oder B komplett.
- Fortlaufende Planung, grafische Wochenansicht, Monat, Serien, Ferien/Feiertage.
- BFV/ICS-Import sowie CSV-Import/-Export.
- Live-Synchronisierung über Firebase Firestore.

## Update auf GitHub Pages
Alle Dateien aus diesem Ordner über die bestehenden Dateien im Repository `svb-platzplan` hochladen und committen. GitHub Pages aktualisiert automatisch.

## Hinweis zum BFV-PDF-Parser
BFV kann das Layout seiner PDF-Exporte ändern. Deshalb zeigt v7 vor dem Import immer eine Prüfliste. Wenn eine konkrete BFV-PDF einmal nicht sauber erkannt wird, kann der Parser anhand genau dieser Datei nachgeschärft werden.
