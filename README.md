<div align="center">

<!-- Typing header -->
[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1200&color=F97316&center=true&vCenter=true&width=720&lines=Hey%2C%20I%27m%20GP%20Singh%20%F0%9F%91%8B%F0%9F%8D%81;AI%20Red-Team%20Engineer%20%F0%9F%A4%96%F0%9F%9B%A1%EF%B8%8F%20Vancouver%20BC;Building%20the%20agentic%20security%20toolkit%20I%20want%20at%20work;Autonomous%20pentest%20pipelines%20%E2%9E%95%20AIxCC-inspired%20CRS;MCP%20servers%20that%20let%20Claude%20drive%20my%20homelab;HTB%20weekends%20%F0%9F%8F%B4%E2%80%8D%E2%98%A0%EF%B8%8F%20AFL%2B%2B%20at%203am%20%F0%9F%A7%A8;Target%3A%20Senior%20AI%20Red%20Team%20%40%20%24200k%20CAD%20by%20Jul%202027)](https://git.io/typing-svg)

<br/>

[![Portfolio](https://img.shields.io/badge/Portfolio-greenbladesec.com-16A34A?style=for-the-badge&logo=safari&logoColor=white)](https://www.greenbladesec.com)
[![Dev.to](https://img.shields.io/badge/Dev.to-Writeups-0A0A0A?style=for-the-badge&logo=dev.to&logoColor=white)](https://dev.to/greenbladesec)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/gpsingh-sec)
[![Visitors](https://komarev.com/ghpvc/?username=PyHackSecGP&color=F97316&style=for-the-badge&label=Profile+Views)](https://github.com/PyHackSecGP)

</div>

---

## 👤 About

```python
profile = {
    "name":         "GP Singh",
    "location":     "Vancouver, BC 🇨🇦",
    "current_role": "Cybersecurity Analyst",
    "target_role":  "Senior AI Red Team Engineer — $200k CAD remote by Jul 2027",
    "thesis":       "LLMs collapse the cost of agentic security tooling — build the stack now",
    "focus": [
        "Agentic security pipelines (ReAct + tool use)",
        "AI red-team / LLM safety eval",
        "SAST/DAST triage + CVE prioritisation",
        "Autonomous HTB / CTF pipelines",
        "Mini-CRS fuzz-to-patch loops (DARPA AIxCC inspired)",
    ],
    "shipped_2026": {
        "projects":    "P1 → P7 end-to-end security tools",
        "mcp_servers": "5 Claude-driven MCPs (cve, wazuh, tooling, ai-redteam, proxmox)",
        "shared_core": "agent-core — ReAct loop used by all P-series projects",
        "tests":       "550+ passing across the portfolio",
    },
    "stack":        ["Python 3.11+", "Claude Haiku + Sonnet", "Ollama", "MCP", "SARIF", "MITRE ATT&CK"],
    "homelab":      "Proxmox + Tailscale mesh + Forgejo mirror + Wazuh + Greenbone + Falco",
    "philosophy":   "Ship over plan. One commit beats a hundred TODOs.",
}
```

---

## 🎯 Portfolio Architecture

```mermaid
graph LR
    subgraph "P-series — security projects"
        P1[P1<br/>SAST+DAST<br/>Triage]
        P2[P2<br/>Threat Model<br/>Generator]
        P3[P3<br/>Log Anomaly<br/>Detector]
        P4[P4<br/>Mini CRS<br/>AFL++→patch]
        P5[P5<br/>ATLAS<br/>Autonomous<br/>Pentest]
        P6[P6<br/>Council<br/>5-persona<br/>Briefings]
        P7[P7<br/>AutoPatch<br/>DD→ZFS→Trivy]
    end
    AC[agent-core<br/>shared ReAct loop]
    subgraph "MCP servers — Claude Desktop tools"
        M1[cve-mcp<br/>NVD+KEV+EPSS]
        M2[wazuh-mcp<br/>SIEM triage]
        M3[tooling-mcp<br/>nmap/nuclei/ffuf]
        M4[ai-redteam-mcp<br/>LLM guardrails]
        M5[proxmox-mcp<br/>VM/LXC ops]
    end
    CLAUDE((Claude<br/>Desktop))
    AC --> P1 & P2 & P3 & P4 & P5
    P5 --> CTF[ctf-lab writeups]
    P4 --> SARIF[SARIF export]
    P7 --> DD[DefectDojo]
    M1 & M2 & M3 & M4 & M5 --> CLAUDE
    style P5 fill:#F97316,color:#fff
    style P4 fill:#F97316,color:#fff
    style AC fill:#7C3AED,color:#fff
    style CLAUDE fill:#D97757,color:#fff
```

---

## 🚀 Featured Projects — The P-Series

| Project | Role | Tests | Stack |
|---|---|---|---|
| [**P5 — ATLAS**](https://github.com/PyHackSecGP/p5-atlas) | 9-agent autonomous HTB pentester with dynamic routing, human checkpoints, tiered Haiku/Sonnet, MITRE ATT&CK writeup, portfolio metrics | **194** | Agentic AI · nmap · ffuf · nuclei · hydra |
| [**P4 — Mini CRS**](https://github.com/PyHackSecGP/p4-mini-crs) | DARPA-AIxCC-inspired: fuzz → ASan triage → LLM root cause → auto-patch → verify. 1-shot CLI + auto daemon. | **121** | AFL++ · Claude Haiku 4.5 · SARIF |
| [**P1 — SAST/DAST Triage**](https://github.com/PyHackSecGP/p1-sast-dast-triage) | Dedupes Semgrep/Bandit/ZAP/Trivy/Nuclei, CWE-based risk scoring, LLM FP filter, SARIF export | **117** | Python · agent-core · Ollama |
| [**P7 — AutoPatch**](https://github.com/PyHackSecGP/p7-autopatch) | Autonomous CVE remediation: DefectDojo → ZFS snapshot → apt/apk patch → Trivy verify → auto-rollback. Zero cloud deps. | **40** | DefectDojo · ZFS · Trivy · systemd |
| [**P3 — Log Anomaly Detector**](https://github.com/PyHackSecGP/p3-log-anomaly-detector) | Rule + z-score detection on auth/journalctl/nginx logs. MITRE ATT&CK heatmap, agentic Ollama investigation, dry-run remediation. Zero third-party deps. | **64** | Python stdlib · Ollama · SARIF |
| [**P2 — Threat Model Generator**](https://github.com/PyHackSecGP/p2-threat-model-generator) | STRIDE from YAML/OpenAPI/Dockerfile/Compose/K8s/Terraform. Compliance flagging (GDPR, PCI-DSS, SOC2, HIPAA). HTML + SARIF reports. | **54** | STRIDE · python-hcl2 · Ollama |

<details>
<summary><b>+ Supporting portfolio (agent-core, CTF lab, MCPs, labs)</b></summary>

| Repo | What it does |
|---|---|
| [agent-core](https://github.com/PyHackSecGP/agent-core) | Shared ReAct tool-calling loop + `@tool` decorator + `ExecutionPolicy` + Claude/Ollama providers. One abstraction, 5 consumers (P1–P5). |
| [cve-mcp](https://github.com/PyHackSecGP/cve-mcp) | MCP unifying NVD + CISA KEV + FIRST EPSS for CVE triage. Composite risk scoring. |
| [wazuh-mcp](https://github.com/PyHackSecGP/wazuh-mcp) | MCP for Wazuh SIEM — NL triage of alerts, agent status, rule lookup. |
| [tooling-mcp](https://github.com/PyHackSecGP/tooling-mcp) | MCP wrappers for nmap / nuclei / gobuster / ffuf / httpx / semgrep / trivy. |
| [ai-redteam-mcp](https://github.com/PyHackSecGP/ai-redteam-mcp) | MCP for LLM guardrail testing — prompt-injection corpus, mutations, bypass tracking. |
| [proxmox-mcp](https://github.com/PyHackSecGP/proxmox-mcp) | MCP for Proxmox VE — list/start/stop VMs + LXCs from Claude Desktop. |
| [ctf-lab](https://github.com/PyHackSecGP/ctf-lab) | Public CTF writeups. ATLAS auto-commits on every successful root. |
| [memory-safety-lab](https://github.com/PyHackSecGP/memory-safety-lab) | C exploitation exercises (buffer overflow, UAF, heap). Intuition training for P4. |
| [offsec-saturdays](https://github.com/PyHackSecGP/offsec-saturdays) | Weekly offensive-security study journal. |

</details>

---

## 📊 GitHub Stats

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=PyHackSecGP&theme=tokyonight&show_icons=true&hide_border=true&count_private=true&include_all_commits=true" />
<img height="165" src="https://github-readme-streak-stats.herokuapp.com?user=PyHackSecGP&theme=tokyonight&hide_border=true" />

<br/>

<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=PyHackSecGP&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" />
<img height="165" src="https://github-profile-trophy.vercel.app/?username=PyHackSecGP&theme=tokyonight&no-frame=true&column=3&row=2&margin-w=10" />

</div>

---

## 🐍 Contribution Snake

<div align="center">

![snake animation](https://raw.githubusercontent.com/PyHackSecGP/PyHackSecGP/output/github-contribution-grid-snake-dark.svg#gh-dark-mode-only)
![snake animation](https://raw.githubusercontent.com/PyHackSecGP/PyHackSecGP/output/github-contribution-grid-snake.svg#gh-light-mode-only)

</div>

---

## ✍️ Latest Writeups

<!-- BLOG-POST-LIST:START -->- [I gave my STRIDE threat modelling tool an agentic interview mode](https://dev.to/greenbladesec/i-gave-my-stride-threat-modelling-tool-an-agentic-interview-mode-1dao) &nbsp; <sub>Sep 2, 2026</sub>- [I Built an AI Security Agent That Found Vulnerabilities in Its Own Code &lpar;And Why That&#39;s the Point&rpar;](https://dev.to/greenbladesec/i-built-an-ai-security-agent-that-found-vulnerabilities-in-its-own-code-and-why-thats-the-point-519h) &nbsp; <sub>Sep 1, 2026</sub>- [Building an AI-Powered Auth Log Anomaly Detector with MITRE ATT&amp;CK](https://dev.to/greenbladesec/building-an-ai-powered-auth-log-anomaly-detector-with-mitre-attck-4ai2) &nbsp; <sub>Aug 31, 2026</sub>- [I Built a SAST/DAST Triage Pipeline Because Scanner Noise Was Killing My Signal](https://dev.to/greenbladesec/i-built-a-sastdast-triage-pipeline-because-scanner-noise-was-killing-my-signal-4126) &nbsp; <sub>Aug 31, 2026</sub>- [Homelab Day: Nextcloud + Traefik + HSTS Headers That Actually Work](https://dev.to/greenbladesec/homelab-day-nextcloud-traefik-hsts-headers-that-actually-work-4cb3) &nbsp; <sub>Aug 11, 2026</sub><!-- BLOG-POST-LIST:END -->

> ⚡ Auto-updated from [dev.to/greenbladesec](https://dev.to/greenbladesec) by a GitHub Action.

---

## 🛠️ Tech Stack

<div align="center">

**Languages & Runtime**  
![Python](https://img.shields.io/badge/Python_3.11+-3776AB?style=flat-square&logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Kali](https://img.shields.io/badge/Kali_Linux-557C94?style=flat-square&logo=kali-linux&logoColor=white)

**AI x Security**  
![Claude](https://img.shields.io/badge/Claude_Haiku+Sonnet-D97757?style=flat-square&logo=anthropic&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama_Local-000?style=flat-square&logo=ollama&logoColor=white)
![MCP](https://img.shields.io/badge/MCP_Protocol-7C3AED?style=flat-square&logoColor=white)
![Agentic](https://img.shields.io/badge/Agentic_ReAct-00A67E?style=flat-square&logoColor=white)
![Prompt Caching](https://img.shields.io/badge/Prompt_Caching-6b4bff?style=flat-square&logoColor=white)

**Offensive**  
![Burp](https://img.shields.io/badge/Burp_Suite-FF6633?style=flat-square&logo=burpsuite&logoColor=white)
![Nmap](https://img.shields.io/badge/Nmap-0E83CD?style=flat-square&logo=nmap&logoColor=white)
![Metasploit](https://img.shields.io/badge/Metasploit-E34F26?style=flat-square&logo=metasploit&logoColor=white)
![ZAP](https://img.shields.io/badge/OWASP_ZAP-00549E?style=flat-square&logo=owasp&logoColor=white)
![AFL++](https://img.shields.io/badge/AFL++_Fuzz-CC0000?style=flat-square&logoColor=white)
![ASan](https://img.shields.io/badge/AddressSanitizer-8B0000?style=flat-square&logoColor=white)

**Defensive**  
![Semgrep](https://img.shields.io/badge/Semgrep-1B2733?style=flat-square&logo=semgrep&logoColor=white)
![Wazuh](https://img.shields.io/badge/Wazuh_SIEM-005F84?style=flat-square&logoColor=white)
![Greenbone](https://img.shields.io/badge/Greenbone-00B388?style=flat-square&logoColor=white)
![Trivy](https://img.shields.io/badge/Trivy-1904DA?style=flat-square&logo=trivy&logoColor=white)
![Falco](https://img.shields.io/badge/Falco-00B4C8?style=flat-square&logo=falco&logoColor=white)
![SARIF](https://img.shields.io/badge/SARIF_2.1.0-333?style=flat-square&logoColor=white)
![MITRE](https://img.shields.io/badge/MITRE_ATT%26CK-C00?style=flat-square&logoColor=white)

**Infra & Ops**  
![Proxmox](https://img.shields.io/badge/Proxmox-E57000?style=flat-square&logo=proxmox&logoColor=white)
![Tailscale](https://img.shields.io/badge/Tailscale_Mesh-000?style=flat-square&logo=tailscale&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![systemd](https://img.shields.io/badge/systemd-FCC624?style=flat-square&logoColor=black)
![Forgejo](https://img.shields.io/badge/Forgejo_Mirror-FB923C?style=flat-square&logoColor=white)
![DefectDojo](https://img.shields.io/badge/DefectDojo-005F84?style=flat-square&logoColor=white)

</div>

---

## 🏴‍☠️ HTB Portfolio Metrics

<div align="center">

![HTB](https://img.shields.io/badge/HackTheBox-9FEF00?style=flat-square&logo=hackthebox&logoColor=black)
![Pipeline](https://img.shields.io/badge/Driver-P5_ATLAS_autonomous_pipeline-F97316?style=flat-square)
![Writeups](https://img.shields.io/badge/Writeups-ctf--lab_auto--committed-16A34A?style=flat-square)

</div>

> P5 ATLAS appends every attempt to `~/.atlas/portfolio.json` — solve rate, duration, MITRE technique histogram, agents involved. Run `python -m metrics` locally for the dashboard. Public writeups land in [ctf-lab](https://github.com/PyHackSecGP/ctf-lab).

---

## 🔭 What I'm Shipping Now

- **P6 Council** — 5-persona AI briefing (voice + text) at 07:00 + 19:00 Pacific — ongoing accountability loop
- **Nudger** — 5x/day Telegram accountability bot with loss-framed messaging, SQLite + nightly CouchDB vault rollup
- **MCP toolkit expansion** — hardening the 5 shipped MCPs (cve, wazuh, tooling, ai-redteam, proxmox) + planning a 6th for SIEM playbook execution
- **ATLAS portfolio metrics** — just added flag-capture tracking + atlas-stats CLI
- **AIxCC-track learning** — reading the full DARPA AIxCC winners' postmortems, folding ideas into P4 Mini-CRS Phase 6

---

## 🧠 How I Work

```
┌─────────────────────────────────────────────────────────────────────┐
│  1. Ship something every day — one function > a hundred TODOs       │
│  2. 3-audience READMEs (novice → interviewer → technical) on every  │
│     portfolio repo so one click is enough to understand the project │
│  3. Tests pass or it doesn't land — 550+ pytests across the P-series│
│  4. Local-first — Ollama fallback on every LLM path. No cloud lock  │
│  5. Zero cloud deps where stdlib covers it (P3 ships with just that)│
│  6. SARIF 2.1.0 + MITRE ATT&CK on everything defender-facing        │
└─────────────────────────────────────────────────────────────────────┘
```

---

## 🏠 Homelab Stack

```
Proxmox 8   ─┬─ PVE host (Tailscale mesh)
             ├─ brain LXC          — CouchDB + Obsidian LiveSync + RSS
             ├─ claw-core (base)   — P4/P6/nudger/stock-tracker systemd
             ├─ mediaserver LXC    — Jellyfin + Seerr + Immich
             ├─ scanner / greenbone — vuln pipeline → DefectDojo
             ├─ pihole / adguard   — DNS + ad filter
             └─ forgejo (Docker)   — self-hosted git mirror of everything
```

ISP router handles LAN perimeter. OPNsense decommissioned 2026-10-28 to simplify the stack.

---

## 🌐 Reach me

<div align="center">

[![Website](https://img.shields.io/badge/greenbladesec.com-16A34A?style=for-the-badge&logo=safari&logoColor=white)](https://www.greenbladesec.com)
[![Dev.to](https://img.shields.io/badge/dev.to%2Fgreenbladesec-0A0A0A?style=for-the-badge&logo=devdotto&logoColor=white)](https://dev.to/greenbladesec)
[![LinkedIn](https://img.shields.io/badge/linkedin.com%2Fin%2Fgpsingh--sec-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/gpsingh-sec)

</div>

<div align="center">

---

<em>"Ship something every day. Consistency beats perfection."</em>

<sub>README driven by GitHub Actions: snake animation (Platane/snk), dev.to post feed (gautamkrishnar/blog-post-workflow). Last authored 2026-10-29.</sub>

</div>
