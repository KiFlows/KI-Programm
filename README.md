# KI für kleine KMU — von 0 zur funktionierenden Architektur

> Das Begleit-Repo zum KiFlows-Programm:  — Stack: Langdock + Claude + Cowork + Obsidian.
> Ansatz: **Architektur zuerst, dann Automatisierung.** Wir bauen mit dir, nicht für dich.

![Architektur](Architektur.svg)

## 🎯 Was du in diesem Programm lernst

1. **Die 3 Schichten deines KI-Systems** — Workspace (immer aktiv), Skills (Wissen bei Bedarf), Agenten (erledigen Aufgaben). Und warum diese Trennung dein System schnell, günstig und wartbar hält.
2. **Agenten richtig schneiden** — pro Aufgabe ein Spezialist (`rechnung-erstellen`, nicht „der Büro-Agent"). Einzige Ausnahme: Orchestratoren wie `Marketing`, die nur delegieren.
3. **Workflow vs. Agent unterscheiden** — kannst du die Schritte vorher aufschreiben, ist es ein Workflow. Das spart echtes Geld: Agenten kosten ~4×, Orchestrator-Systeme ~15× so viele Tokens wie ein Chat.
4. **Sauber delegieren** — der Delegations-Vertrag (Ziel · Fakten · Format · Grenzen), damit Subagenten nicht raten müssen.
5. **Sicherheit von Anfang an** — Least Privilege: Jeder Agent bekommt nur die Rechte, die seine Aufgabe braucht. Whitelist statt Blacklist, kein Hard-Delete durch KI, nach außen geht nichts ohne deine Freigabe.
6. **Ehrliche KI** — keine erfundenen Preise, Zahlen oder Studien. Fakten kommen aus deinen Skills, alles andere wird nachgefragt. Das ist in jedem Agenten fest verdrahtet.
7. **Selbst weiterbauen** — mit dem `agent-builder` erstellst du nach dem Programm eigene Agenten, die sich an alle Regeln halten.

## 📦 Was du am Ende hast

| Sektion | Agenten | Skills |
|---|---|---|
| [[00_Base_Config/README\|00 Basis]] | Skill-Manager | ueber-mich, firma-ueber, firma-brand-voice, firma-produkte |
| [[01_Basic_Agents/README\|01 Basis-Agenten]] | agent-builder · ablage-suchen · dokument-erstellen · ablage-pflegen | firma-ablage |
| [[02_Recherche_Wissen/README\|02 Recherche]] | recherche-bericht (+ täglicher Workflow ⏰) | firma-domain |
| [[03_Marketing/README\|03 Marketing]] | Marketing (Orchestrator) → linkedin-post · insta-post · blog-artikel · video-script | 4 Format-Skills |
| [[04_Vertrieb_Kunden/README\|04 Vertrieb]] | kunden-recherche · angebot-erstellen · follow-up-email | firma-angebotsvorlage |
| [[05_Finanzen/README\|05 Finanzen]] | rechnung-erstellen · zahlungserinnerung | firma-rechnungsdaten |
| [[06_Backoffice/README\|06 Backoffice]] | meeting-protokoll | protokoll-format |

Alles systemneutral: dieselben Templates funktionieren in Langdock, ChatGPT und Claude — die `Anpassung.md` in jedem Agenten-Ordner regelt die Unterschiede.

## 🧭 So arbeitest du mit dem Repo

Pro Sektion genau zwei Einstiege: **`00_Anleitung.md`** (Checkliste — damit arbeitest du live) und **`00_Dokumentation.md`** (Theorie zum Nachlesen). Jeder Agent hat seinen Ordner: `Agent_<name>.md` (fertiges Template) + `Anpassung.md` (Fragen + System-/Business-Anpassung) + ggf. `Skill_*.md`.

---

