# SVB Platzplan v5

Mobile PWA für die Platz- und Terminplanung der Fußballabteilung des SV Buckenhofen.

## Neu in v5
- **C-Platz ergänzt:** zusätzliche halbe Trainingsfläche ohne Tore; bewusst nur für Training / Notfallbelegung
- A- und B-Platz bleiben jeweils halbierbar; Spiele/Turniere belegen weiterhin A oder B komplett
- **Fortlaufende Planung:** In der detaillierten Planung werden beim Herunterscrollen automatisch weitere Tage nachgeladen
- **Fortlaufende grafische Ansicht:** In der horizontalen Tagesübersicht werden beim Wischen nach rechts automatisch weitere Tage nachgeladen
- Wochenpfeile bleiben als schneller Sprung um ±1 Woche erhalten; „Heute“ setzt die fortlaufende Ansicht zurück
- C-Flächennutzung wird im Wochenüberblick mit ausgewertet

## Aus v4 weiterhin enthalten
- Mo–Fr 14:00–22:00 Uhr, Sa/So 09:00–22:00 Uhr
- Pflichtfeld „Trainer / verantwortlich“, Bearbeiter separat im Änderungsprotokoll
- Terminbezeichnung optional; automatische Beschreibung aus Mannschaft + Terminart
- Trainerzuordnung pro Mannschaft im Adminbereich
- BFV/ICS-Import, CSV-Import und CSV-Export im Adminbereich
- Serientermine mit Saison-Presets Herbst/Winter/Sommer; einzelne Termine und Serie ab einem Termin löschbar
- Bayerische Schulferien 2026/27 und gesetzliche Feiertage als Planungsinfo
- Monatsansicht, Live-Synchronisierung und Konfliktprüfung

## Hinweis zu Berechtigungen
Der Adminbereich wird aktuell anhand des lokal hinterlegten Namens ein-/ausgeblendet. Das ist bewusst eine einfache Vereinslösung und noch keine sicherheitstechnisch harte Rollensteuerung. Für den breiten Rollout sollte optional eine Admin-PIN oder echte Authentifizierung ergänzt werden.
