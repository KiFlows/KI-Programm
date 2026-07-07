# 📖 Dokumentation — Wissen zum Nachlesen

Hintergrundwissen zur [[00_Start_Anleitung|Start-Anleitung]]. Hier gibt es nichts abzuarbeiten — lies einen Abschnitt, wenn die Anleitung dich hierher schickt.

**Inhalt:**
1. [Skill-Sprache](#skill-sprache) — in welcher Sprache schreibe ich Skills?
2. [Negative Regeln](#negative-regeln) — was die KI NICHT tun darf
3. [Typische Fehler](#typische-fehler) — die 5 häufigsten Stolperfallen

---

## Skill-Sprache

### Deutsch, Englisch — oder egal?

> **Merksatz: Mechanik englisch. Stimme in der Sprache deines Outputs.**

**Die Faustregel:**

🔧 **Technische Skills & Agenten-Regeln → Englisch**
Logik, Trigger, „wie baue ich einen Skill" — das befolgt das Modell minimal zuverlässiger.

🗣️ **Voice- & Inhalts-Skills → deine Zielsprache**
Brand Voice, Über-mich, alles wo am Ende deutscher Text rauskommt — in genau dieser Sprache schreiben.

**Warum?** KI-Modelle sind überwiegend mit englischen Daten trainiert. Englische Anweisungen werden minimal genauer befolgt — ABER: soll deutscher Text entstehen, helfen deutsche Beispiele & Ton mehr als Englisch. Der Effekt ist real, aber klein. Kein Grund zur Panik — Hauptsache konsistent.

**Für dein Setup heißt das:**

| Element | Sprache |
|---|---|
| Skill-Manager / Agenten-Regeln | Englisch |
| Workspace-Mechanik | Englisch oder Deutsch |
| Brand Voice | Zielsprache (z.B. Deutsch) |
| Über mich / Über die Firma | Zielsprache |
| `description` / Trigger | egal — Mischung ok |

**Eine Sache bleibt immer gleich:** Der interne Name (slug) ist technisch und ändert sich NIE — englisch/kebab-case, in jeder Sprache. Nur sichtbarer Name + Inhalt richten sich nach der Sprache.

> Schreib die **Regeln** auf Englisch.
> Schreib die **Persönlichkeit** in deiner Sprache.

---

## Negative Regeln

Negative Regeln sind genauso wichtig wie positive. Sie verhindern, dass die KI selbstbewusst Dinge erfindet.

Beispiele, die in fast jeden Agenten gehören:

- „Erfinde keine Preise."
- „Nenne keine Garantien."
- „Verwende keine Buzzwords wie revolutionär, disruptiv, game-changing."
- „Wenn Informationen fehlen, frage nach."
- „Keine automatischen Kundenversprechen ohne Freigabe."

> Die wichtigste Regel ist die letzte im Beispielblock: **Fehlende Info → nachfragen statt raten.**

---

## Typische Fehler

Die größten Risiken sind nicht technisch, sondern organisatorisch:

1. **Zu viele Agenten zu früh**
   Dann weiß niemand mehr, welchen Agenten man wofür nutzt. Lieber wenige, klar benannte Agenten am Anfang.

2. **Skills ohne klare Grenzen**
   Wenn Skills Marketing, Preise, Prozesse und Tonalität vermischen, wird es schnell chaotisch. Ein Thema = ein Skill.

3. **Agenten als „magische Alles-Könner" bauen**
   Besser: kleine spezialisierte Agenten mit klarer Aufgabe — nach Aufgabe benannt („LinkedIn Post Builder"), nicht nach Rolle („Marketing Bot").

4. **Keine Single Source of Truth**
   Produktinfos, Preise, Brand Claims und Prozesse müssen aus Skills/Knowledge kommen — nicht aus dem Modellgedächtnis. Und jede Info nur an EINEM Ort.

5. **Automatisierung ohne Review-Schritt**
   Gerade bei Kundenkommunikation, Angeboten, Social Media: erst assistieren, dann automatisieren.
