<!--
  ══════════════════════════════════════════════════════════════════
  ANIKA KOTHARI -GitHub profile README -EDITING GUIDE (hidden)
  ══════════════════════════════════════════════════════════════════
  This whole guide is an HTML comment -invisible when rendered on
  GitHub, visible only when you (or future-you) open this file to edit.

  COLOR TOKENS
    black  #050505   white  #F5F5F5   purple #B026FF
    lime   #C8FF00   grey   #8a8a8a

  PAGE STRUCTURE
    hero.svg  → nav badges → About → System Log → Projects
    (Active Build, then Shipped) → Stack → Contact

  REUSABLE CHROME
    assets/winbar.svg  -the dark strip with 3 dots + "SYSTEM ONLINE"
    that sits above every "##" heading. Just drop
    <img src="assets/winbar.svg" width="100%" /> above any new section
    heading to match the look. Don't edit the SVG itself -it has no
    text baked in that needs changing.

    assets/divider.svg -thin gradient rule used for breathing room
    between major blocks.

  ── ADD A SYSTEM LOG ROW (was "Experience") ──────────────────────
  It's a plain markdown table now -just add a row:
  | 20XX·MON–MON | Role -Organization | tag1 · tag2 |

  ── ADD A "SHIPPED" PROJECT CARD ─────────────────────────────────
  Copy one <td>...</td> block between the PROJECT CARD START/END
  markers below, paste into a <tr>, edit the contents. Two <td>s
  per <tr>. Use `[ HW ]` or `[ SW ]` (or your own tag) as the
  category marker up front so the hardware/software mix stays
  visible at a glance.

  ── ADD AN "ACTIVE BUILD" (ongoing project) ──────────────────────
  Ongoing work lives above Shipped, tagged with the
  STATUS-ACTIVE BUILD badge instead of a repo link. Copy the Techy
  Bhai block (the smaller of the two Active Build entries) as your
  template -it doesn't need a custom diagram. Only give a project
  the full NeerAI treatment (own SVG flow diagram) if it's your
  actual flagship; otherwise the small-card format is enough.

  ── MOVE SOMETHING FROM ACTIVE BUILD → SHIPPED ───────────────────
  Once it's done: swap the STATUS badge for a "REPO →" badge, and
  move the block down into the Shipped table.

  ── STACK TABLE ───────────────────────────────────────────────────
  One <tr> per category. Edit the `·`-separated list in the second
  <td>. Add "(learning)" after anything not solid yet.
  ══════════════════════════════════════════════════════════════════
-->

<div align="center">

<img src="assets/hero.svg" width="100%" alt="Anika Kothari -electronics × software × AI" />

<sub><i>learning never hits exit, only run.</i></sub>

<br><br>

<a href="#about"><img src="https://img.shields.io/badge/NAV-ABOUT-B026FF?style=for-the-badge&labelColor=050505" /></a>
<a href="#system-log"><img src="https://img.shields.io/badge/NAV-LOG-C8FF00?style=for-the-badge&labelColor=050505" /></a>
<a href="#projects"><img src="https://img.shields.io/badge/NAV-PROJECTS-B026FF?style=for-the-badge&labelColor=050505" /></a>
<a href="#stack"><img src="https://img.shields.io/badge/NAV-STACK-C8FF00?style=for-the-badge&labelColor=050505" /></a>
<a href="#contact"><img src="https://img.shields.io/badge/NAV-CONTACT-B026FF?style=for-the-badge&labelColor=050505" /></a>

<br><br>

<a href="[GITHUB_URL]"><img src="https://img.shields.io/badge/GITHUB-050505?style=for-the-badge&logo=github&logoColor=C8FF00" /></a>
<a href="[LINKEDIN_URL]"><img src="https://img.shields.io/badge/LINKEDIN-050505?style=for-the-badge&logo=linkedin&logoColor=B026FF" /></a>
<a href="mailto:[EMAIL]"><img src="https://img.shields.io/badge/EMAIL-050505?style=for-the-badge&logo=gmail&logoColor=C8FF00" /></a>
<a href="[RESUME_URL]"><img src="https://img.shields.io/badge/OPEN-RESUME-B026FF?style=for-the-badge&labelColor=050505" /></a>

</div>

<br>

<img src="assets/winbar.svg" width="100%" />

## About

<table width="100%">
<tr>
<td width="140" valign="top">

<sub><b>ROLE</b></sub><br>
<sub><b>FOCUS</b></sub><br>
<sub><b>LOOP</b></sub><br>
<sub><b>BASED</b></sub>

</td>
<td valign="top">

3rd year,Btech, Electronics and Computer Science Engg.<br>
software systems and applied AI, with a real embedded/hardware foundation underneath<br>
Plan → Code → Test → Optimize<br>
SRM Institute of Science & Technology, Chennai, India

</td>
</tr>
</table>

Equally comfortable writing the firmware that reads a sensor and the pipeline that decides what to do with what it read. Recent work sits at that seam -safety research on software-defined vehicles, fault injection in simulation, ECU and kill-switch circuits on an actual kart, and AI systems that never touch hardware at all. Same instinct either way: find where the signal is lying to you, then fix it.

<br>

<img src="assets/divider.svg" width="100%" />

<br>

<img src="assets/winbar.svg" width="100%" />

## System Log

<!-- add a row: | 20XX·MON–MON | Role -Organization | tag1 · tag2 | -->

| TIME | PROCESS | TAGS |
|:--|:--|:--|
| `2026 · MAY–JUL` | SDV & AI Automotive Safety Research Intern -IIT Indore | SDV · SOTIF · Rust · STM32F407 |
| `2026 · FEB–PRESENT` | Electrical & Firmware -Team Full Throttle (GKDC Kart) | C/C++ · ECU integration · kill-switch design |
| `2026 · MAY–JUN` | Research Intern -Open Knowledge Initiatives × IIIT-H | SPARQL · Wikidata · OCR pipelines |
| `2025 · JUL–PRESENT` | Committee Member, Sponsorship & Mgmt -Aaruush | corporate pitching · MoUs |
| `2025 · DEC` | Industrial Trainee -Pi-Tech India (MSME Certified) | Arduino · ESP32 · UART/I2C/SPI |

<br>

<img src="assets/divider.svg" width="100%" />

<br>

<img src="assets/winbar.svg" width="100%" />

## Projects

<img src="https://img.shields.io/badge/-ACTIVE%20BUILD-C8FF00?style=flat-square&labelColor=050505" /> &nbsp;<sub>currently running</sub>

<div align="center">

**`[ FEATURED ]`**

### NEERAI -water-stress-aware compute scheduling

<img src="assets/neerai-flow.svg" width="100%" />

</div>

Data centres get sited and scheduled around latency and cost -almost never around water. NeerAI adds regional water stress as a real scheduling variable, not a footnote, and routes compute accordingly.

**what it does** -profiles workloads, predicts resource pressure, and runs a multi-objective optimizer (`J = αC + βE + γWs + δL`) across compute, energy, and water stress before a job ever gets placed.

**what's built so far** -the optimizer, a Python digital-twin harness for simulating infrastructure telemetry, and a routing layer that turns four competing variables into one decision. Still actively evolving.

`Python` · `XGBoost` · `optimization` · `digital twins` · `telemetry`

<img src="https://img.shields.io/badge/STATUS-ACTIVE%20BUILD-C8FF00?style=for-the-badge&labelColor=050505" />
<a href="[NEERAI_REPO]"><img src="https://img.shields.io/badge/VIEW-REPOSITORY-B026FF?style=for-the-badge&labelColor=050505" /></a>

<br>

<table width="100%">
<tr>

<!-- PROJECT CARD START -->
<td width="100%" valign="top">

**`[ SW ]` TECHY BHAI**
<sub>micro-learning platform</sub>

Full-stack platform delivering personalized tech content through a recommendation engine, with JWT + Google OAuth auth and a MySQL schema built around a user-interest graph.

`Next.js` `Node.js` `Express` `MySQL`

<img src="https://img.shields.io/badge/STATUS-IN%20PROGRESS-B026FF?style=flat-square&labelColor=050505" />
<a href="[TECHYBHAI_REPO]"><img src="https://img.shields.io/badge/REPO-→-B026FF?style=flat-square&labelColor=050505" /></a>

</td>
<!-- PROJECT CARD END -->

</tr>
</table>

<br>

<img src="https://img.shields.io/badge/-SHIPPED-8a8a8a?style=flat-square&labelColor=050505" /> &nbsp;<sub>done, working, out in the world</sub>

<!--
  PROJECT CARD TEMPLATE -copy one <td>...</td> block, paste into a <tr>, edit contents.
  Two <td> cells per <tr>. Add a new <tr> for every 2 new projects.
-->

<table width="100%">
<tr>

<!-- PROJECT CARD START -->
<td width="50%" valign="top">

**`[ HW ]` RAILSENTINALS**
<sub>track safety & hazard detection · SIH 2025 National Finalist</sub>

AI-vision + sensor fusion system for automated railway track defect monitoring. ESP32 nodes process ballast health and obstacle telemetry in real time; loco-aware braking logic computes emergency stopping distances on hazard detection.

`ESP32` `Embedded C++` `Computer Vision` `Python`

<a href="[RAILSENTINALS_REPO]"><img src="https://img.shields.io/badge/REPO-→-B026FF?style=flat-square&labelColor=050505" /></a>

</td>
<!-- PROJECT CARD END -->

<!-- PROJECT CARD START -->
<td width="50%" valign="top">

**`[ SW ]` NEWSZ**
<sub>graph-based news exploration engine</sub>

Converts unstructured news into a navigable knowledge graph -custom adjacency-list structures, binary-heap priority queues, and Union-Find powering Dijkstra's and Kruskal's traversal modes, with LLM-based keyword extraction on top.

`JavaScript (ES6+)` `Graphs` `Union-Find` `LLM APIs`

<a href="[NEWSZ_REPO]"><img src="https://img.shields.io/badge/REPO-→-C8FF00?style=flat-square&labelColor=050505" /></a>

</td>
<!-- PROJECT CARD END -->

</tr>
<tr>

<!-- PROJECT CARD START -->
<td width="50%" valign="top">

**`[ HW ]` AGRITECH**
<sub>closed-loop sensor controller</sub>

ESP32-based closed-loop controller processing real-time soil-moisture telemetry to trigger automated irrigation cycles. Implemented software hysteresis to kill relay chatter and cut power draw.

`ESP32` `Embedded C++` `Hardware Control`

<a href="[AGRITECH_REPO]"><img src="https://img.shields.io/badge/REPO-→-B026FF?style=flat-square&labelColor=050505" /></a>

</td>
<!-- PROJECT CARD END -->

<!-- PROJECT CARD START -->
<td width="50%" valign="top">

**`[ SW ]` ASCENDRA**
<sub>AI-driven career roadmap platform</sub>

Cross-platform app that treats skill growth like a dependency graph. LLM APIs generate adaptive roadmaps and missions with stateful context across sessions; Firebase handles real-time sync and auth.

`Flutter` `Firebase` `LLM APIs`

<a href="[ASCENDRA_REPO]"><img src="https://img.shields.io/badge/REPO-→-C8FF00?style=flat-square&labelColor=050505" /></a>

</td>
<!-- PROJECT CARD END -->

</tr>
<tr>

<!-- PROJECT CARD START -->
<td width="100%" valign="top" colspan="2">

**`[ SW ]` ADVERA**
<sub>blockchain ad-settlement & fraud resolution</sub>

Off-chain Python engine using Merkle-tree inclusion proofs to verify ad-impression records, with Solidity contracts that process submission hashes on-chain and auto-flag disputed activity.

`Solidity` `Python` `MySQL` `Merkle Trees`

<a href="[ADVERA_REPO]"><img src="https://img.shields.io/badge/REPO-→-C8FF00?style=flat-square&labelColor=050505" /></a>

</td>
<!-- PROJECT CARD END -->

</tr>
</table>

<br>

<sub><b>FIELD NOTES</b></sub>

`[2025]` SIH National Finalist -RailSentinals, AI-vision track hazard monitoring system
`[2026]` IIT Indore -SDV / SOTIF safety research
`[2026]` OKI × IIIT-H -performance stipend, cohort of ~140
`[——]` National Spelling Bee -3rd place

<br>

<img src="assets/divider.svg" width="100%" />

<br>

<img src="assets/winbar.svg" width="100%" />

## Stack

<!-- one <tr> per category. Edit the `·`-separated list. Add "(learning)" for anything not solid yet. -->

<table width="100%">
<tr><td width="170"><sub><b>LANGUAGES</b></sub></td><td>Python · C · C++ · JavaScript (ES6+) · SQL · Solidity · Rust <sub>(foundations)</sub></td></tr>
<tr><td><sub><b>WEB & BACKEND</b></sub></td><td>React · Node.js · Express · REST APIs · JWT · Google OAuth · HTML/CSS</td></tr>
<tr><td><sub><b>AI & AUTOMOTIVE</b></sub></td><td>ML Fundamentals · LLM APIs · SOTIF · SDV Architectures · CARLA · LGSVL · NVIDIA DRIVE Sim · IPG CarMaker</td></tr>
<tr><td><sub><b>EMBEDDED & HARDWARE</b></sub></td><td>STM32F407 · ESP32 · Arduino · CAN / UART / SPI / I2C · Digital Twins · OTA Updates</td></tr>
<tr><td><sub><b>TOOLS & INFRA</b></sub></td><td>Git · MySQL · Firebase · Linux · Docker <sub>(learning)</sub> · Microservices <sub>(learning)</sub></td></tr>
</table>

<br>

<img src="assets/divider.svg" width="100%" />

<br>

<img src="assets/winbar.svg" width="100%" />

<div align="center" id="contact">

## Contact

Building NeerAI, applying elsewhere, always open to the interesting kind of problem.

<a href="[GITHUB_URL]"><img src="https://img.shields.io/badge/GITHUB-050505?style=for-the-badge&logo=github&logoColor=C8FF00" /></a>
<a href="[LINKEDIN_URL]"><img src="https://img.shields.io/badge/LINKEDIN-050505?style=for-the-badge&logo=linkedin&logoColor=B026FF" /></a>
<a href="mailto:[EMAIL]"><img src="https://img.shields.io/badge/EMAIL-050505?style=for-the-badge&logo=gmail&logoColor=C8FF00" /></a>

</div>

<br>
