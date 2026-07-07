# Prompt — Infos extrahieren (mit Links)

> Nutze diesen Prompt, **wenn deine KI GitHub-Seiten lesen kann** (siehe Test 2 in der Start-Anleitung). Sonst → `Prompt_InfosExtrahieren_Anhang.md`.

## Prompt
- [ ] Erledigt

>DE
```kopieren
Du kennst mich aus unseren bisherigen Chats und deinem Memory.
Die Vorlagen liegen öffentlich auf GitHub. Hole sie dir selbst — ich hänge nichts an und lade nichts herunter.

Vorlagen (per Raw-URL abrufen):
- https://raw.githubusercontent.com/KiFlows/KI-Programm/main/Skill_ueber-mich.md
- https://raw.githubusercontent.com/KiFlows/KI-Programm/main/Skill_firma-ueber.md
- https://raw.githubusercontent.com/KiFlows/KI-Programm/main/Skill_firma-markenstimme.md
- https://raw.githubusercontent.com/KiFlows/KI-Programm/main/Skill_firma-produkte.md
- https://raw.githubusercontent.com/KiFlows/KI-Programm/main/Workspace.md

Ablauf:
1. Rufe jede der fünf Raw-URLs ab und lies die Vorlage als Ausgangsstruktur ein.
2. Fülle jede Vorlage einzeln aus — nutze ALLES, was du schon über mich, meine Firma und meine Schreibweise weißt.

Ausgabe:
- Wenn du Dateien erstellen kannst: gib jede ausgefüllte Vorlage als eigene .md-Datei aus (gleicher Dateiname wie die Vorlage).
- Wenn nicht: gib jede ausgefüllte Vorlage als EINEN kopierbaren Markdown-Code-Block aus, Dateinamen als Textzeile darüber — eines nach dem anderen.

Regeln:
- Behalte den Kopf jeder Vorlage (die drei Zeilen Interner Name / Sichtbarer Name / Beschreibung) und fülle die Werte aus. Keinen YAML-Block daraus machen.
- In den Kopfzeilen NUR die Platzhalter [Name] / [Firma] durch die echten Werte ersetzen — sonst nichts ändern. Übersetze keine Eigen- oder Firmennamen (Cristina bleibt Cristina, „My Dream" bleibt „My Dream").
- Der Inhalt (alles unter der Linie) wird durchgehend in EINER Sprache geschrieben: Deutsch. Ausnahme: Eigennamen, Firmennamen und feststehende Begriffe bleiben original.
- Ersetze JEDEN [ ]-Platzhalter durch echte Werte und entferne die eckigen Klammern. Im Ergebnis dürfen keine [ ] mehr stehen — außer [BITTE ERGÄNZEN].
- Wo dir Infos fehlen: NICHT raten. Schreibe [BITTE ERGÄNZEN] und stelle mir am Ende EINE gebündelte Frageliste über alle Vorlagen hinweg.
- Ändere die Struktur (Überschriften, die drei Kopf-Felder) nicht.
- Für firma-markenstimme: leite meinen Ton daraus ab, wie ICH dir in unseren Chats geschrieben habe — nicht aus generischen Annahmen.
- Bei firma-produkte: nur Fakten, kein Marketing. Was du nicht sicher weißt → [BITTE ERGÄNZEN].

Besonderheiten:
- Skill_ueber-mich.md: schreibe hier ALLES rein, was du über mich weißt — ausführlich.
- Workspace.md hat drei Teile, alle kurz halten (immer aktiv):
  - Unternehmensbeschreibung — Kurzbeschreibung der Firma (1 Satz).
  - About me (kurz) — die wichtigsten Punkte über mich (Doppelung mit ueber-mich ist ok).
  - Model Instructions — diesen Teil auf ENGLISCH schreiben. Wie ich mit den Agents arbeite (Ton mir gegenüber, Widerspruch erwünscht, Nachfragen vor großen Aktionen, Sprache, Format). Das ist NICHT Brand Voice (= Außenauftritt) — leite es da