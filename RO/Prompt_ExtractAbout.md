Mă cunoști din conversațiile noastre anterioare și din memoria ta.
Șabloanele sunt publice pe GitHub. Adu-le singur — nu atașez și nu descarc nimic.

Șabloane (preia prin raw URL, repo KiFlows/KI-Programm, branch main):
- https://raw.githubusercontent.com/KiFlows/KI-Programm/main/RO/Skill_about-me.md
- https://raw.githubusercontent.com/KiFlows/KI-Programm/main/RO/Skill_firma-about.md
- https://raw.githubusercontent.com/KiFlows/KI-Programm/main/RO/Skill_firma-brand-voice.md
- https://raw.githubusercontent.com/KiFlows/KI-Programm/main/RO/Skill_firma-produkte.md
- https://raw.githubusercontent.com/KiFlows/KI-Programm/main/RO/Workspace.md

Pași:
1. Preia fiecare dintre cele cinci URL-uri raw și citește șablonul ca structură de bază.
2. Completează fiecare șablon individual — folosește TOT ce știi deja despre mine, compania mea și stilul meu de scris.

Output:
- Dacă poți crea fișiere: returnează fiecare șablon completat ca fișier .md propriu (același nume ca șablonul).
- Dacă nu: returnează fiecare șablon completat ca UN singur bloc de cod Markdown copiabil, cu numele fișierului ca linie de text deasupra — unul după altul.

Reguli:
- Păstrează antetul fiecărui șablon (cele trei linii **Nume intern** / **Nume vizibil** / **Descriere**) și completează valorile. Nu transforma în bloc YAML.
- În liniile de antet înlocuiește DOAR placeholder-ele [Nume] / [Companie] cu valorile reale — nu schimba nimic altceva. Nu traduce nume proprii sau de companie (Cristina rămâne Cristina, „My Dream" rămâne „My Dream").
- Conținutul (tot ce e sub linie) se scrie integral într-o SINGURĂ limbă: română. Excepție: nume proprii, nume de companie și termeni consacrați rămân în original.
- Înlocuiește FIECARE placeholder [ ] cu valori reale și elimină parantezele. Nu trebuie să mai rămână niciun [ ] — cu excepția [DE COMPLETAT].
- Unde lipsesc informații: NU ghici. Scrie [DE COMPLETAT] și dă-mi la final O singură listă grupată de întrebări pentru toate șabloanele.
- Nu schimba structura (titluri, cele trei câmpuri de antet).
- Pentru firma-brand-voice: deduce tonul meu din felul în care ȚI-am scris în conversațiile noastre — nu din presupuneri generice.
- Pentru firma-produkte: doar fapte, fără marketing. Ce nu știi sigur → [DE COMPLETAT].

Particularități:
- Skill_about-me.md: scrie aici TOT ce știi despre mine — în detaliu.
- Workspace.md are trei părți, păstrează-le scurte (mereu active):
  - **Descrierea companiei** — descriere scurtă a companiei (1 propoziție).
  - **Despre mine (pe scurt)** — cele mai importante puncte despre mine (suprapunerea cu about-me e ok).
  - **Instrucțiuni pentru model** — cum lucrez cu agenții (tonul față de mine, dezacordul binevenit, întreabă înainte de acțiuni mari, limbă, format). Aceasta NU este vocea brandului (= prezentarea externă) — deduce din felul în care îți scriu în conversații și ce îmi doresc.

Dacă un URL nu poate fi preluat: spune-mi exact care, în loc să ghicești.
