<!--
╔══════════════════════════════════════════════════════════════════════════════╗
║  NEBELREBELL · GITHUB PROFILE README                                         ║
║  FiveM / QB-Core Development · IT Automation · Applied AI                    ║
╚══════════════════════════════════════════════════════════════════════════════╝
-->

<!-- ── Blaue Wellen-Leiste (oben am Rand) ────────────────────────────────────── -->
<p align="center">
  <img
    src="https://capsule-render.vercel.app/api?type=waving&height=120&color=0:0f172a,50:0369a1,100:0ea5e9"
    alt=""
    width="100%"
  />
</p>

<!-- ── Logo ──────────────────────────────────────────────────────────────────── -->
<p align="center">
  <a href="https://nebelbank.net">
    <img
      src="https://nebelbank.net/de/Gemini_Generated_Image_cxqrmbcxqrmbcxqr.png"
      alt="NebelRebell · Nebelbank.net"
      width="260"
    />
  </a>
</p>

<!-- ── Schriftzug mit Farbverlauf ────────────────────────────────────────────── -->
<p align="center">
  <img
    src="https://capsule-render.vercel.app/api?type=transparent&height=80&color=0:0ea5e9,50:38bdf8,100:0369a1&text=%F0%9F%91%8B%20HeyHey%2C%20I%27m%20NebelRebell&fontColor=0ea5e9&fontSize=44&fontAlign=50&fontAlignY=52&animation=fadeIn"
    alt="👋 HeyHey, I'm NebelRebell"
    width="100%"
  />
</p>

<h3 align="center">
  FiveM-Script-Developer ·
  Community Founder &amp; Manager of the Multigaming Community
  <a href="https://nebelbank.net">Nebelbank.net</a> since 1997 ·
  Creative Streamer &amp; Gaming Pioneer since the C64 / Amiga 500 era
</h3>

<p align="center"><strong>[WIP] Nebelbank.net – Legacy RP – Back to the Roots</strong></p>

<p align="center">
  <a href="https://github.com/nebelrebell">
    <img
      src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&pause=1200&color=0EA5E9&center=true&vCenter=true&width=760&lines=Community+Founder+%26+Manager+%40+Nebelbank.net;Multigaming+Community+since+1997;Building+production-grade+FiveM+%2F+QB-Core+resources;Automating+everything+that+runs+twice;Bringing+AI+into+real+developer+workflows"
      alt="Focus areas"
    />
  </a>
</p>

<p align="center">
  <a href="https://nebelbank.net"><img src="https://img.shields.io/badge/Nebelbank.net-Founder_%26_Manager-0ea5e9?style=for-the-badge&logo=firefoxbrowser&logoColor=white" alt="Nebelbank.net" /></a>
  <a href="https://discord.gg/scg3YqZFU6"><img src="https://img.shields.io/badge/Discord-Join-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>
  <a href="https://www.youtube.com/c/nebelbanknet"><img src="https://img.shields.io/badge/YouTube-Channel-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="YouTube" /></a>
  <a href="https://instagram.com/nebelbanknet"><img src="https://img.shields.io/badge/Instagram-Follow-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram" /></a>
  <a href="https://linktr.ee/nebelbanknet"><img src="https://img.shields.io/badge/Linktree-All_Links-39E09B?style=for-the-badge&logo=linktree&logoColor=white" alt="Linktree" /></a>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=nebelrebell&label=Profile+Views&color=0ea5e9&style=flat-square" alt="Profile views" />
  <img src="https://img.shields.io/github/followers/nebelrebell?label=Followers&style=flat-square&color=0ea5e9&logo=github" alt="Followers" />
  <img src="https://img.shields.io/github/stars/nebelrebell?label=Stars&style=flat-square&color=eab308&logo=github" alt="Stars" />
</p>

---

## `01` — About

**Founder and Manager of the Multigaming Community [Nebelbank.net](https://nebelbank.net) — since 1997.**

I have been building, breaking and rebuilding systems since the **C64 / Amiga 500** era. Today my work
sits at the intersection of three disciplines that turn out to reinforce each other remarkably well:

| Domain | What I actually do |
| :--- | :--- |
| **FiveM · QB-Core** | Server-authoritative resources, framework-level integrations, OneSync-safe state handling, performance budgets that survive a full server. |
| **IT Automation** | Deployment pipelines, scripted server operations, monitoring and self-healing infrastructure — removing every task that repeats. |
| **Applied AI** | LLM-assisted development workflows, agent tooling and automation that produces reviewable, production-ready output — not demos. |

> [!NOTE]
> **Current project — `Nebelbank.net · Legacy RP · Back to the Roots`** *(WIP)*
> A roleplay server built on the principle that stability and fair play beat feature bloat.

<br />

## `02` — Engineering Principles

Every resource I ship is measured against the same four gates. This is the flow a script goes through
before it ever reaches a live server:

```mermaid
flowchart LR
    A["💡 Concept"] --> B["🏗️ Server-Authoritative<br/>Design"]
    B --> C["🔒 Trust Boundary<br/>Review"]
    C --> D["⚡ Performance<br/>Budget"]
    D --> E["🤖 Automated<br/>Deployment"]
    E --> F["✅ Production"]
    C -.->|"client input<br/>never trusted"| B
    D -.->|"over budget"| B

    classDef node fill:#0ea5e9,stroke:#0369a1,stroke-width:2px,color:#ffffff;
    classDef done fill:#16a34a,stroke:#15803d,stroke-width:2px,color:#ffffff;
    class A,B,C,D,E node;
    class F done;
```

<details>
<summary><b>What each gate means in practice</b> — click to expand</summary>

<br />

**Server-Authoritative Design** — the client renders, the server decides. Money, inventory, jobs and
state transitions are validated server-side, always. No exceptions for convenience.

**Trust Boundary Review** — every `RegisterNetEvent` is treated as a public, hostile API. Payloads are
type-checked, rate-limited and bound to the caller's actual source. Events that mutate state are never
callable without validation.

**Performance Budget** — resources are profiled under load, not on an empty server. Threads run at the
lowest viable tick rate, loops exit early, and `Citizen.Wait(0)` is justified or removed.

**Automated Deployment** — no manual file copying, no "it works on my server". Reproducible builds,
scripted rollouts, verifiable rollbacks.

</details>

<br />

## `03` — Stack

<table align="center">
<tr>
<td align="center" width="33%">

**Core Development**

<img src="https://skillicons.dev/icons?i=lua,js,ts,html,css&theme=dark" height="40" alt="Lua, JavaScript, TypeScript, HTML, CSS" />

</td>
<td align="center" width="33%">

**Data & Infrastructure**

<img src="https://skillicons.dev/icons?i=mysql,mariadb,linux,docker,nginx&theme=dark" height="40" alt="MySQL, MariaDB, Linux, Docker, Nginx" />

</td>
<td align="center" width="33%">

**Tooling & Workflow**

<img src="https://skillicons.dev/icons?i=git,github,vscode,bash,powershell&theme=dark" height="40" alt="Git, GitHub, VS Code, Bash, PowerShell" />

</td>
</tr>
</table>

<p align="center">
  <img src="https://img.shields.io/badge/FiveM-F40552?style=flat-square&logo=fivem&logoColor=white" alt="FiveM" />
  <img src="https://img.shields.io/badge/QB--Core-0ea5e9?style=flat-square" alt="QB-Core" />
  <img src="https://img.shields.io/badge/ESX-1e293b?style=flat-square" alt="ESX" />
  <img src="https://img.shields.io/badge/ox__lib-334155?style=flat-square" alt="ox_lib" />
  <img src="https://img.shields.io/badge/OneSync-475569?style=flat-square" alt="OneSync" />
  <img src="https://img.shields.io/badge/txAdmin-64748b?style=flat-square" alt="txAdmin" />
  <img src="https://img.shields.io/badge/LLM_Agents-7c3aed?style=flat-square&logo=openaigym&logoColor=white" alt="LLM Agents" />
</p>

<br />

## `04` — GitHub Activity

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api?username=nebelrebell&show_icons=true&hide_border=true&theme=tokyonight&bg_color=00000000&title_color=0ea5e9&icon_color=0ea5e9&text_color=94a3b8" />
  <source media="(prefers-color-scheme: light)" srcset="https://github-readme-stats.vercel.app/api?username=nebelrebell&show_icons=true&hide_border=true&bg_color=00000000&title_color=0369a1&icon_color=0369a1&text_color=334155" />
  <img src="https://github-readme-stats.vercel.app/api?username=nebelrebell&show_icons=true&hide_border=true&theme=transparent&title_color=0ea5e9&icon_color=0ea5e9" height="165" alt="GitHub statistics" />
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=nebelrebell&layout=compact&hide_border=true&theme=tokyonight&bg_color=00000000&title_color=0ea5e9&text_color=94a3b8&langs_count=8" />
  <source media="(prefers-color-scheme: light)" srcset="https://github-readme-stats.vercel.app/api/top-langs/?username=nebelrebell&layout=compact&hide_border=true&bg_color=00000000&title_color=0369a1&text_color=334155&langs_count=8" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=nebelrebell&layout=compact&hide_border=true&theme=transparent&title_color=0ea5e9&langs_count=8" height="165" alt="Most used languages" />
</picture>

<br /><br />

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-streak-stats.herokuapp.com/?user=nebelrebell&hide_border=true&background=00000000&stroke=1e293b&ring=0ea5e9&fire=0ea5e9&currStreakLabel=0ea5e9&sideLabels=94a3b8&dates=64748b&currStreakNum=e2e8f0&sideNums=e2e8f0" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=nebelrebell&hide_border=true&background=00000000&stroke=cbd5e1&ring=0369a1&fire=0369a1&currStreakLabel=0369a1&sideLabels=334155&dates=64748b" height="165" alt="Contribution streak" />
</picture>

<br /><br />

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-activity-graph.vercel.app/graph?username=nebelrebell&theme=react-dark&bg_color=00000000&color=0ea5e9&line=0ea5e9&point=e2e8f0&area=true&area_color=0ea5e9&hide_border=true&custom_title=Contribution%20Activity" />
  <source media="(prefers-color-scheme: light)" srcset="https://github-readme-activity-graph.vercel.app/graph?username=nebelrebell&bg_color=00000000&color=0369a1&line=0369a1&point=1e293b&area=true&area_color=0ea5e9&hide_border=true&custom_title=Contribution%20Activity" />
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=nebelrebell&theme=react-dark&bg_color=00000000&hide_border=true" alt="Contribution activity graph" width="100%" />
</picture>

</div>

<br />

## `05` — Contribution Snake

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/nebelrebell/nebelrebell/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/nebelrebell/nebelrebell/output/github-snake.svg" />
  <img src="https://raw.githubusercontent.com/nebelrebell/nebelrebell/output/github-snake.svg" alt="Snake eating my contribution graph" width="100%" />
</picture>

</div>

<br />

## `06` — Support

<div align="center">

<a href="https://www.buymeacoffee.com/nebelrebell">
  <img src="https://img.shields.io/badge/Buy_Me_A_Coffee-Support_the_work-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black" alt="Buy Me A Coffee" />
</a>

<br /><br />

<img
  src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=15&pause=1500&color=64748B&center=true&vCenter=true&width=640&lines=Every+coffee+becomes+a+new+QB-Core+resource;...open-source+tooling+for+the+FiveM+community;...and+keeps+Nebelbank.net+running+since+1997"
  alt="Support impact"
/>

</div>

---

<div align="center">

<img
  src="https://capsule-render.vercel.app/api?type=soft&height=110&color=0:0f172a,50:0369a1,100:0ea5e9&text=The%20Power%20of%20Perfection&fontColor=ffffff&fontSize=30&fontAlign=50&fontAlignY=48&desc=Don't%20flame%20without%20brain%20%C2%B7%20Your%20satisfaction%20is%20our%20achievement&descAlign=50&descAlignY=76&descSize=13&animation=twinkling"
  alt="The Power of Perfection"
  width="100%"
/>

<br />

<code>#FiveM</code> · <code>#QBCore</code> · <code>#Lua</code> · <code>#Roleplay</code> ·
<code>#ITAutomation</code> · <code>#AI</code> · <code>#OpenSource</code> · <code>#Nebelbank</code>

<br /><br />

<a href="https://github.com/nebelrebell"><img src="https://img.shields.io/badge/↑_Back_to_top-0ea5e9?style=for-the-badge" alt="Back to top" /></a>

</div>

<p align="center">
  <img
    src="https://capsule-render.vercel.app/api?type=transparent&height=50&color=0:0ea5e9,100:0369a1&text=Thanks%20for%20stopping%20by&fontColor=64748b&fontSize=18&fontAlign=50&fontAlignY=50&animation=fadeIn"
    alt="Thanks for stopping by"
    width="100%"
  />
</p>

<!-- ── Blaue Wellen-Leiste (unten am Rand) ───────────────────────────────────── -->
<img
  src="https://capsule-render.vercel.app/api?type=waving&section=footer&height=120&color=0:0ea5e9,50:0369a1,100:0f172a"
  alt=""
  width="100%"
/>
