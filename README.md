# KI-Programm: Langdock
Public documents needed for the KI Programm 


## Langdock Settings
### Workspace_Unternehmensbeschreibung
> Schlank halten — dieser Text ist in *jedem* Chat aktiv und kostet Kontext.

##### Ersetze "Firma"
> Frontmatter-Konvention (Langdock): `slug` = Identifier, `name` = sichtbarer Name.
>- Beispiel slug: about-kiflows
>- name: KI Flows — brand reference

 **Regel:** 
- Maximal ~5–8 Zeilen echter Inhalt.
- Keine Details, die nur für bestimmte Outputs nötig sind.
##### was hier NICHT hingehört
- Alles, was nur *manchmal* gebraucht wird (Rechtsform, Signatur, Verträge), gehört NICHT hierher, sondern in den about-firma Skill.

---
# SKILLS
> Naming: persönlich = `about-me`, firmenbezogen = `firma-*` (Firma zuerst): `firma-about`, `firma-brand-voice`, `firma-produkte`.

## Skill_about-me
Persönliche Referenz: Rolle, Expertise, Hintergrund, Sprachen, Arbeitsweise.
**Regel:** Nur die Person — keine Firmendaten (→ firma-about), kein Ton (→ firma-brand-voice).

---

## Skill_firma-about

##### Ersetze "Firma"
>- Beispiel slug: about-kiflows

**Regel:** 
- Hier kommt die **detaillierte Referenz** rein, die nur für bestimmte Outputs gebraucht wird
 (E-Mails, Angebote, Verträge, rechtliche Texte, Positionierung).
 - Pro Firma ein eigener Skill: `about-kiflows`, `about-websmartik`, ...

##### was hier NICHT hingehört
- Tagesaktueller Grundton/1-Zeiler → der gehört ins **Workspace** (immer aktiv).
- Ton & Sprachregeln → `firma-brand-voice`.
- Produktdetails & Preise → `firma-produkte`, nicht hier vermischen.

---

## Skill_firma-brand-voice


###### Self-Check vor dem Veröffentlichen

- Frage: [z.B. „Würde ein skeptischer Kunde mit den Augen rollen?" Wenn ja → neu schreiben.]

---

## Skill_firma-produkte
**Zweck:** Fakten über Angebote, Preise und Pakete.
Wichtig: **Dieser Skill sollte faktisch sein, nicht werblich.**

Warum getrennt vom Brand Skill?  
Weil Preise und Produktdetails sich häufiger ändern als Tonalität.

---
# AGENTS


