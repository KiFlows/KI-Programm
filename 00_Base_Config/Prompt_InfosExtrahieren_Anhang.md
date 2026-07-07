# Prompt — Infos extrahieren (mit Anhang)

> Nutze diesen Prompt, **wenn deine KI keine GitHub-Seiten lesen kann** (Test 2 fehlgeschlagen). Lade die 5 Vorlagen von GitHub herunter und **hänge sie an** (mit +), dann diesen Prompt einfügen.
> Download: https://github.com/KiFlows/KI-Programm

## Prompt
- [ ] Erledigt

>DE
```kopieren
Du kennst mich aus unseren bisherigen Chats und deinem Memory.
Ich habe dir mehrere Vorlagen als Dateien angehängt (Skill_ueber-mich, Skill_firma-ueber, Skill_firma-markenstimme, Skill_firma-produkte, Workspace).

Ablauf:
1. Lies jede angehängte Vorlage als Ausgangsstruktur ein.
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
  - Model Instructions — diesen Teil auf ENGLISCH schreiben. Wie ich mit den Agents arbeite (Ton mir gegenüber, Widerspruch erwünscht, Nachfragen vor großen Aktionen, Sprache, Format). Das ist NICHT Brand Voice (= Außenauftritt) — leite es daraus ab, wie ich dir in unseren Chats schreibe und was ich mir wünsche.

Falls eine Vorlage fehlt: sag mir genau welche, statt zu raten.
```

> [!code]- English version (Klicke zum Ausklappen)
> ```kopieren
> You know me from our previous chats and your memory.
> I have attached several templates as files (Skill_ueber-mich, Skill_firma-ueber, Skill_firma-markenstimme, Skill_firma-produkte, Workspace).
>
> Steps:
> 1. Read each attached template as the base structure.
> 2. Fill in each template individually — use EVERYTHING you already know about me, my company and my writing style.
>
> Output:
> - If you can create files: return each filled template as its own .md file (same filename as the template).
> - If not: return each filled template as ONE copyable Markdown code block, with the filename as a text line above it — one after another.
>
> Rules:
> - Keep each template's header (the three lines Internal name / Visible name / Description) and fill in the values. Do not turn it into a YAML block.
> - In the header lines, replace ONLY the placeholders [Name] / [Company] with the real values — change nothing else. Do not translate personal or company names (Cristina stays Cristina, "My Dream" stays "My Dream").
> - The content (everything below the line) is written entirely in ONE language: German. Exception: proper names, company names and established terms stay original.
> - Replace EVERY [ ] placeholder with real values and remove the brackets. No [ ] may remain — except [BITTE ERGÄNZEN].
> - Where info is missing: do NOT guess. Write [BITTE ERGÄNZEN] and give me ONE bundled question list across all templates at the end.
> - Do not change the structure (headings, the three header fields).
> - For firma-markenstimme: derive my tone from how I have written to you in our chats — not from generic assumptions.
> - For firma-produkte: facts only, no marketing. What you are not sure about → [BITTE ERGÄNZEN].
>
> Specifics:
> - Skill_ueber-mich.md: write EVERYTHING you know about me here — in detail.
> - Workspace.md has three parts, keep all short (always active):
>   - Company description — short description of the company (1 sentence).
>   - About me (short) — the most important points about me (overlap with ueber-mich is ok).
>   - Model Instructions — write this part in ENGLISH. How I work with the agents (tone toward me, disagreement welcome, ask before big actions, language, format). This is NOT brand voice (= external) — derive it from how I write to you in our chats and what I want.
>
> If a template is missing: tell me exactly which one, instead of guessing.
> ```
