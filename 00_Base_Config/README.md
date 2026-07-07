# KI-Programm: Langdock

Öffentliche Vorlagen für das KI-Programm. **Starte hier:** [`00_Start_Anleitung.md`](00_Start_Anleitung.md) — Schritt-für-Schritt-Checkliste mit allen Links.

---
## Die 3 Schichten
1. **Workspace** — kurze Infos, in *jedem* Chat aktiv. → `Workspace.md`
2. **Skills** — Detailwissen, lädt nur *bei Bedarf*. → `Skill_*.md`
3. **Agenten** — erledigen Aufgaben, nutzen Skills. → `Agent_*.md`

## Dateien

**Anleitung 
- `00_Start_Anleitung.md` — der Einstieg, Checkliste mit Links
- `00_Dokumentation.md` — Wissen zum Nachlesen (Skill-Sprache, Negative Regeln, Typische Fehler)

**Prompts (kopierst DU manuell)**
- [[Prompt_InfosExtrahieren.md]]— Vorlagen füllen lassen (KI holt sie per Link von GitHub)
- [[Prompt_InfosExtrahieren_Anhang.md]] — Fallback: Vorlagen anhängen statt verlinken
- [[Prompt_SkillsHinzufuegen.md]] — gefüllte Vorlagen an den Skill-Manager übergeben

**Vorlagen für Deine Skills (liest die KI, füllt sie aus)**
- [[Skill_ueber-mich.md]]
- [[Skill_firma-ueber.md]]
- [[Skill_firma-markenstimme.md]] 
- [[Skill_firma-produkte.md]]
- [[Workspace.md]] — die immer-aktiven Kurztexte

**Beispiele KI Flows skills**
- [[Beispiel_BrandVoice_kiflows.md]] — ausgefülltes Beispiel

**Agenten (kopierst DU in Langdock)**
- [[Agent_00_Skill-Manager.md]] — erstellt/aktualisiert Skills

## Konventionen

**Die drei Werte** ( jeder Skill-Vorlage):
· **Interner Name** (kebab-case, sprachneutral, z.B. `firma-about`) 
· **Sichtbarer Name** (Anzeigename, z.B. „Über Cristina") 
· **Beschreibung** (wann laden + Negativ-Abgrenzung).


**Benennung:** 
- persönlich = `about-me` ·
- firmenbezogen = `firma-*` (Firma zuerst): 
  Beispiel: `firma-about`, `firma-brand-voice`, `firma-produkte`.

**Format:** 
- Anleitung, Prompts und Agenten haben **1-Klick-Kopierblöcke** (```kopieren```) und die andere Sprache als **ausklappbare** Alternative. 
- Die fünf Vorlagen (`Skill_*`, `Workspace`) bleiben bewusst **schlicht ohne Kopierblöcke** — die KI liest sie direkt per Link/Anhang, da würde Extra-Formatierung stören.

**Workspace ≠ Skill:** 
Immer-relevant → Workspace. 
Nur-manchmal-nötig → Skill. 
Ton → `firma-markenstimme` (nie im Workspace). 
Produkte/Preise → `firma-produkte`.
