# 🚀 Start-Anleitung — KI mit Langdock einrichten

Diese Anleitung führt dich Schritt für Schritt durch die Einrichtung. Du arbeitest die Checkliste von oben nach unten ab — jeder Schritt hat den passenden Link.

**Wichtige Links:**
- Langdock: https://app.langdock.com
- GitHub (alle Vorlagen): https://github.com/KiFlows/KI-Programm
- Obsidian: https://obsidian.md
- 📖 Hintergrundwissen zum Nachlesen: [[00_Dokumentation]]

> [!tip] Die 3 Schichten, die wir bauen
> 1. **Workspace** — kurze Infos, in *jedem* Chat aktiv (Firma + du in Kurzform).
> 2. **Skills** — Detailwissen, lädt nur *bei Bedarf* (über dich, Firma, Brand Voice, Produkte).
> 3. **Agenten** — erledigen Aufgaben und nutzen die Skills.
>
> **Faustregel:** Immer relevant → Workspace. Nur manchmal nötig → Skill. (Zu viele immer geladene Infos kosten Credits.)

---

## Teil A — Langdock kennenlernen

### A1 · Langdock öffnen
- [ ] Erledigt
- Gehe zu 👉 https://app.langdock.com (oder Registrierung: https://app.langdock.com/signup)

### A2 · Chat testen
- [ ] Erledigt
- Einen einfachen Chat starten und oben das **Modell wechseln** (z.B. Claude ↔ GPT).

### A3 · Workspace-Einstellungen ansehen (noch NICHT ändern)
- [ ] Erledigt
- Langdock → **Workspace-Einstellungen**. Diese Punkte ansehen:
  - Individuelle Anweisungen
  - Allgemein → Unternehmensbeschreibung & Logo
  - Erinnerung → **aktivieren**
  - Nutzung
  - Modelle

---

## Teil B — Skills verstehen

### B1 · Zwei fertige Skills freigeben
- [ ] Erledigt
- Langdock → **Skills**. Diese zwei aktivieren: **Skill Creator** und **Platform Help**.

> [!info]+ Was ist ein Skill?
> Ein wiederverwendbares Wissens- und Regelpaket, das deine KI nutzt — z.B. „über mich", „Firma", „Brand Voice", „Produkte".

> [!info]+ Triggering
> Ein Skill wird nur geladen, wenn er relevant ist (Triggering). Daraus folgt die saubere Aufteilung: ein Thema = ein Skill.

> [!info]+ Klare Grenzen = der Trigger
> Die Beschreibung sagt, *wann* der Skill lädt. Beispiel: „Nutze diesen Skill, wenn du ein Angebot, eine Leistungsbeschreibung oder eine Preisaussage für unser Unternehmen erstellst."

> [!info]+ Single Source of Truth
> Jede Info nur an EINEM Ort. Denselben „truth" in mehreren Skills (Beschreibungen) zu definieren verwirrt den Agent und ist unperformant. Produktinfos, Preise, Brand Claims und Prozesse kommen aus Skills/Knowledge — nicht aus Modellgedächtnis, Anweisungen oder Memory.

> [!info]+ Warum Skill statt PDF?
> **Ein Skill ist eine Anweisung, die befolgt wird. Ein Wissensdokument ist ein Fakt, der gesucht wird.**
> Ein Skill wird **ganz** geladen → zuverlässig. Ein PDF/Wissensdokument wird **durchsucht** (RAG) → kann Infos verfehlen. Firma & Brand Voice willst du *ganz geladen* → also Skill, nicht PDF.

---

## Teil C — Deine Infos vorbereiten (das Herzstück)

Bevor du Vorlagen ausfüllen lässt: **zwei kurze Tests** mit deiner KI (z.B. ChatGPT). Sie entscheiden, welchen Weg du gehst.

### ✅ Test 1 — Kennt dich deine KI? (Memory)
- [ ] Erledigt
- Diesen Prompt in deine KI einfügen:

>DE
```kopieren
Gib mir alles, was du über mich und meine Firma weißt. Fasse es zusammen.
```

> [!code]- English version (Klicke zum Ausklappen)
> ```kopieren
> Give me everything you know about me and my company. Summarize it.
> ```

- **Kommt etwas Sinnvolles?** → weiter zu Test 2.
- **Kommt nichts / nur Allgemeines?** → deine KI hat **kein** Wissen über dich. Dann diesen Weg:
  - Lade jede Vorlage **einzeln in Langdock** hoch, erzähl der KI über dich, lass die Vorlage füllen.
  - Für die **Brand Voice**: lade 3–5 eigene E-Mails hoch → dein Ton wird daraus abgeleitet.

### ✅ Test 2 — Kann deine KI GitHub lesen? (Browsing)
- [ ] Erledigt
- Diesen Prompt in deine KI einfügen:

>DE
```kopieren
Öffne diese Seite und sag mir die erste Überschrift, die du siehst: https://raw.githubusercontent.com/KiFlows/KI-Programm/main/Skill_ueber-mich.md
```

> [!code]- English version (Klicke zum Ausklappen)
> ```kopieren
> Open this page and tell me the first heading you see: https://raw.githubusercontent.com/KiFlows/KI-Programm/main/Skill_ueber-mich.md
> ```

- **Sie liest es korrekt?** → nimm **`Prompt_InfosExtrahieren.md`** (Version mit Links).
- **Sie kann nicht / erfindet etwas?** → lade die Vorlagen von GitHub herunter, **hänge sie an** und nimm **`Prompt_InfosExtrahieren_Anhang.md`** (Version ohne Links).

### C1 · Infos extrahieren
- [ ] Erledigt
- 📖 **Lies vorher:** [[00_Dokumentation#Skill-Sprache|Skill-Sprache]] — in welcher Sprache schreibst du deine Skills? (Kurz: Mechanik englisch, Stimme in deiner Sprache.)
- Passenden Prompt öffnen und in deine KI einfügen:
  - Mit Links: [[Prompt_InfosExtrahieren]]
  - Mit Anhang: [[Prompt_InfosExtrahieren_Anhang]]

### C2 · Ergebnis prüfen
- [ ] Erledigt
- Alle **`[BITTE ERGÄNZEN]`** füllen. Fakten, Preise und Signatur **selbst kontrollieren** — die KI rät sonst.

---

## Teil D — Skills in Langdock anlegen

### D1 · Skill-Manager-Agent erstellen
- [ ] Erledigt
- Langdock → **Agenten** → neuer Agent. Vorlage: [[Agent_00_Skill-Manager|Agent Skill Manager]]
- 📖 **Lies dazu:** [[00_Dokumentation#Negative Regeln|Negative Regeln]] — was deine KI NICHT tun darf, ist genauso wichtig.

### D2 · Skills übergeben
- [ ] Erledigt
- Die ausgefüllten Vorlagen an den Skill-Manager geben. Prompt: [[Prompt_SkillsHinzufuegen|Prompt Skills hinzufügen]]

### D3 · Workspace-Texte einsetzen
- [ ] Erledigt
- Die kurzen Texte aus `Workspace.md` in Langdock einfügen (Unternehmensbeschreibung + Individuelle Anweisungen). Vorlage: [[Workspace]]

---

> [!success] Fertig
> Workspace gefüllt · Skills angelegt · Agenten aktiv. Deine KI kennt jetzt dich, deine Firma und deinen Ton.

> [!warning] Bevor du weiterbaust
> 📖 Lies die [[00_Dokumentation#Typische Fehler|5 typischen Fehler]] — die größten Risiken sind nicht technisch, sondern organisatorisch.

---

## 📝 Hausaufgabe

Lies in Ruhe durch, was die KI über dich geschrieben hat, und korrigiere es. Offene `[BITTE ERGÄNZEN]`-Stellen füllen.

### Teil 1 — Workspace kontrollieren (immer aktiv)
- [ ] **Über mich (kurz)** — stimmen die wichtigsten Punkte? Kurz halten.
- [ ] **Unternehmensbeschreibung (Company)** — 1 Satz, korrekt und aktuell?
- [ ] **Model Instructions** — passt, wie die KI mit dir arbeiten soll?

> Workspace änderst du direkt in Langdock → Workspace-Einstellungen.

### Teil 2 — Skills kontrollieren (bei Bedarf)
- [ ] **Skill „Über mich"** (about-me) — vollständig und richtig?
- [ ] **Skill „Firma"** (firma-about) — Daten, Signatur, Positionierung korrekt?
- [ ] **Skill „Brand Voice"** (firma-brand-voice) — klingt der Ton wirklich nach dir?
- [ ] **Skill „Produkte"** (firma-produkte) — Pakete, Preise und Status korrekt? Nur Fakten, kein Marketing.

> Skill ändern: Datei anpassen und an den **Skill-Manager-Agenten** geben → er aktualisiert den Skill.
