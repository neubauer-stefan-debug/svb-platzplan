# SVB Platzplan v6

Mobile PWA für die Platz- und Terminplanung der Fußballabteilung des SV Buckenhofen.

## Neu in v6 – einfacher Trainer-Zugang
- Keine Google-Anmeldung und keine E-Mail-Adresse nötig.
- Beim ersten Aufruf: Trainer auswählen und persönliche 4-stellige PIN eingeben.
- Das Gerät merkt den erfolgreichen Login lokal; beim normalen nächsten Start ist keine erneute PIN nötig.
- Wird eine PIN im Adminbereich geändert, muss sie beim nächsten Start neu eingegeben werden.
- Ersteinrichtung: Solange noch keine PIN vergeben ist, kann der erste Admin-Zugang (Stefan) seine Admin-PIN direkt festlegen.
- Admin kann anschließend für Holger, Bülent und weitere Trainer PINs setzen oder ändern sowie neue Zugänge anlegen.
- Rollen: Trainer (nur zugeordnete Mannschaften bearbeiten), Vollzugriff (alle Termine bearbeiten), Admin (zusätzlich Zugänge, Im-/Export, Grundeinstellungen).
- Alle dürfen den gesamten Platzplan sehen.
- Bearbeitername kommt aus dem Login und ist im Termin nicht frei manipulierbar.

## Weiterhin aus v5
- A1/A2, B1/B2 und C-Platz als halbe Trainingsfläche ohne Tore.
- Spiele/Turniere belegen A oder B komplett.
- Fortlaufende Planung und horizontal fortlaufende grafische Wochenansicht.
- Mo–Fr 14:00–22:00 Uhr, Sa/So 09:00–22:00 Uhr.
- Monatsübersicht, Serientermine, Ferien-/Feiertagsinfos, Konfliktprüfung.
- BFV/ICS-Import sowie CSV-Import/-Export im Adminbereich.
- Live-Synchronisierung über Firebase Firestore.

## Erster Start nach dem Update
1. v6 veröffentlichen.
2. App öffnen.
3. `Stefan` auswählen.
4. Neue 4-stellige Admin-PIN zweimal eingeben.
5. Im Adminbereich unter **Zugänge & PINs** PINs für weitere Trainer vergeben.
6. Die Trainer öffnen denselben Link, wählen ihren Namen und melden sich einmal mit ihrer PIN an.

## Sicherheitshinweis
Die PIN-/Rollensteuerung in v6 ist bewusst eine einfache vereinsinterne App-Sperre. Die PIN wird nicht im Klartext gespeichert, sondern als Hash. Die darunterliegende Firebase-Verbindung nutzt weiterhin anonyme Firebase-Authentifizierung. Gegen gezielte technische Manipulation ist dies keine gleichwertige serverseitige Benutzer-/Rollensteuerung. Für einen späteren breiten öffentlichen Rollout kann eine echte Firebase-Benutzeranmeldung ergänzt werden, ohne Google-Login in der Oberfläche zu benötigen.
