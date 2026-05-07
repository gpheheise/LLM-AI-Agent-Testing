# awesome-automated-pentest

> A curated list of automated penetration testing tools — AI-powered agents and traditional script-based automation.
> Focus: web · network · Active Directory. All tools below are open-source, free to use, and self-hostable.

---

## Overview

Two parallel ecosystems are emerging in offensive security automation:

| Track | Description |
|-------|-------------|
| **AI-powered** | LLM-driven agents that reason, plan, and execute exploitation chains autonomously or semi-autonomously |
| **Script-based** | Deterministic wrappers that orchestrate established tools (nmap, NetExec, testssl, etc.) without AI |

This list is a working reference for both. Curated for use in authorised engagements only.

---

## AI-Powered Automated Pentest Tools

### Agentic / Autonomous Frameworks

| Tool | Focus | Stack | License | Repo |
|------|-------|-------|---------|------|
| **PentestGPT** | Web · CTF · multi-domain | Python, agentic pipeline, Docker, 20+ tools | MIT | [GreyDGL/PentestGPT](https://github.com/GreyDGL/PentestGPT) |
| **CAI** (Cybersecurity AI) | Bug bounty · red team · CTF | Python, multi-agent, 300+ model backends, supports Ollama for air-gapped | MIT (research) | [aliasrobotics/cai](https://github.com/aliasrobotics/cai) |
| **PentAGI** | Full-stack autonomous pentest | Multi-agent, Docker sandbox, 20+ tools (nmap, Metasploit, sqlmap…) | Apache 2.0 | [vxcontrol/pentagi](https://github.com/vxcontrol/pentagi) |
| **Strix** | Web app dynamic testing · PoC generation | HTTP proxy, browser automation, terminal, Python exploit env | MIT | [usestrix/strix](https://github.com/usestrix/strix) |
| **RAPTOR** | Code review · binary analysis · exploit + patch | Built on Claude Code, semgrep, CodeQL, fuzzing | MIT | [gadievron/raptor](https://github.com/gadievron/raptor) |
| **Pentest-Swarm-AI** | Multi-agent web/bug bounty | Go, ReAct agents, 7+ native tools, Claude/OpenAI/Ollama | MIT | [Armur-Ai/Pentest-Swarm-AI](https://github.com/Armur-Ai/Pentest-Swarm-AI) |
| **METATRON** | Recon + AI analysis (offline) | Python, Ollama, MariaDB, fully air-gapped | MIT | [sooryathejas/METATRON](https://github.com/sooryathejas/METATRON) |
| **AutoPentest-AI** | Web app · WSTG-aligned | MCP server, parallel pipelines, knowledge graph | MIT | [bhavsec/autopentest-ai](https://github.com/bhavsec/autopentest-ai) |

### MCP-Based (LLM + Tools)

| Tool | Focus | Stack | License | Repo |
|------|-------|-------|---------|------|
| **HexStrike AI** | General offensive (web · network · AD) | MCP server, 150+ tools, multi-agent, works with Claude/GPT/Copilot | MIT | [0x4m4/hexstrike-ai](https://github.com/0x4m4/hexstrike-ai) |
| **Pentest-AI (ptai)** | Web · MCP server | 197+ tools, MCP, browser agent, SARIF/JUnit/PDF reports, scope enforcement | MIT | [0xSteph/pentest-ai](https://github.com/0xSteph/pentest-ai) |
| **Kali MCP** | Generic Kali toolbox via MCP | Dockerized Kali, MCP transport | MIT | [Vasanthadithya-mundrathi/Pentest-MCP](https://github.com/Vasanthadithya-mundrathi/Pentest-MCP) |
| **Hexstrike AI (PL fork)** | Hardened HexStrike with guardrails | Scope validator, blast-radius tiers, kill switch | MIT | [netcuter/Hexstrike-AI](https://github.com/netcuter/Hexstrike-AI) |

### LLM Assistants (Human-in-the-Loop)

| Tool | Focus | Notes | Repo |
|------|-------|-------|------|
| **HackingBuddyGPT** | Linux privesc · SSH | ~50 lines of Python, ReAct loop, ideal as a starting point | [ipa-lab/hackingBuddyGPT](https://github.com/ipa-lab/hackingBuddyGPT) |
| **Nebula** | AI-assisted terminal | Recon · note-taking · CWE/NIST mapping | [berylliumsec/nebula](https://github.com/berylliumsec/nebula) |
| **LLM4Pentest (curated)** | Survey + reading list | Tracks academic + open-source LLM pentest research | [simon-p-j-r/LLM4Pentest](https://github.com/simon-p-j-r/LLM4Pentest) |
| **awesome-cybersecurity-agentic-ai** | Aggregator | Comprehensive list of agentic-AI security projects | [raphabot/awesome-cybersecurity-agentic-ai](https://github.com/raphabot/awesome-cybersecurity-agentic-ai) |

---

## Offline / Non-AI Automated Pentest Tools

### Network & Service Enumeration

| Tool | What It Automates | Repo |
|------|-------------------|------|
| **AutoRecon** | nmap → service-specific enumeration (nikto, gobuster, smbmap, enum4linux, …) | [Tib3rius/AutoRecon](https://github.com/Tib3rius/AutoRecon) |
| **nmapAutomator** | Layered nmap scan (Quick → Full → UDP → Vulns → Recon) | [21y4d/nmapAutomator](https://github.com/21y4d/nmapAutomator) |
| **NetExec (nxc)** | SMB/LDAP/MSSQL/WinRM/RDP/SSH/FTP/WMI exploitation modules | [Pennyw0rth/NetExec](https://github.com/Pennyw0rth/NetExec) |
|

### Active Directory

| Tool | What It Automates | Repo |
|------|-------------------|------|
| **linWinPwn** | Wraps 30+ AD tools (impacket, NetExec, certipy, bloodyAD, kerbrute, lsassy, …) — interactive & automated mode | [lefayjey/linWinPwn](https://github.com/lefayjey/linWinPwn) |
| **ldeep** | In-depth LDAP enumeration: users, GMSA, LAPS, delegations, ADCS, trusts | [franc-pentest/ldeep](https://github.com/franc-pentest/ldeep) |
| **windapsearch** | Python LDAP enumeration of users, groups, computers | [ropnop/windapsearch](https://github.com/ropnop/windapsearch) |
| **enum4linux-ng** | SMB/RPC enumeration, modern rewrite of enum4linux | [cddmp/enum4linux-ng](https://github.com/cddmp/enum4linux-ng) |
| **DonPAPI** | DPAPI secret extraction at scale | [login-securite/DonPAPI](https://github.com/login-securite/DonPAPI) |
| **kerbrute** | User enumeration & password spray via Kerberos pre-auth | [ropnop/kerbrute](https://github.com/ropnop/kerbrute) |

### Web Application

| Tool | What It Automates | Repo |
|------|-------------------|------|
| **Nuclei** | Template-based vulnerability scanning (web, network, DNS, cloud) | [projectdiscovery/nuclei](https://github.com/projectdiscovery/nuclei) |
| **Jaeles** | Signature-based web app scanner framework | [jaeles-project/jaeles](https://github.com/jaeles-project/jaeles) |
| **ZAP Automation Framework** | OWASP ZAP scans driven by YAML, CI-friendly | [zaproxy/zaproxy](https://github.com/zaproxy/zaproxy) |
| **OSTE Meta Scanner** | Combines Nikto, ZAP, Nuclei, SkipFish, Wapiti | [OSTE-Meta-Scan](https://github.com/OSTEsayed/OSTE-Meta-Scanner) |
| **httpx / katana / dnsx** | Fast HTTP probing, crawling, DNS resolution (ProjectDiscovery suite) | [projectdiscovery](https://github.com/projectdiscovery) |

### TLS / Crypto

| Tool | What It Automates | Repo |
|------|-------------------|------|
| **testssl.sh** | TLS/SSL configuration testing, ciphers, vulnerabilities | [drwetter/testssl.sh](https://github.com/drwetter/testssl.sh) |
| **sslscan** | Fast TLS cipher / protocol scanner | [rbsec/sslscan](https://github.com/rbsec/sslscan) |

### Aggregators & Methodology

| Resource | Description | Repo |
|----------|-------------|------|
| **PentestingEverything** | Curated VAPT toolset (web · mobile · API · AD · cloud · …) | [m14r41/PentestingEverything](https://github.com/m14r41/PentestingEverything) |
| **Pentest-Tools (S3cur3Th1sSh1t)** | Massive curated link list, AD-heavy | [S3cur3Th1sSh1t/Pentest-Tools](https://github.com/S3cur3Th1sSh1t/Pentest-Tools) |
| **AD-Pentesting-Tools** | AD-specific tooling reference | [theyoge/AD-Pentesting-Tools](https://github.com/theyoge/AD-Pentesting-Tools) |
| **Awesome PentestTools** | General offensive tooling collection | [arch3rPro/PentestTools](https://github.com/arch3rPro/PentestTools) |

---

## Quick Pick — Where to Start

| Use case | Recommendation |
|----------|----------------|
| Internal AD assessment, no AI | **AutoRecon** + **nmap2nxc** + **linWinPwn** |
| Web app pentest, no AI | **Nuclei** + **Jaeles** + **ZAP Automation** |
| AI-assisted web pentest (cloud LLM) | **Strix** or **CAI** |
| AI-assisted, fully air-gapped | **METATRON** or **CAI** with Ollama backend |
| AI integrated with Claude/Cursor | **HexStrike AI** (MCP) or **RAPTOR** |
| Learning / research base | **HackingBuddyGPT** (~50 LoC ReAct loop) |

---

## Notes

- **Air-gapped operation**: METATRON and CAI explicitly support fully offline LLM use via Ollama. PentestGPT and most MCP servers can be configured with local models, but require manual setup.
- **MCP vs direct tool calling**: MCP-based tools (HexStrike, ptai) need a compatible client (Claude Code, Cursor, VS Code Copilot). Direct-call frameworks (CAI, PentAGI, Strix) are self-contained.
- **Token cost warning**: Long agentic loops (Strix, PentAGI) can consume 50M+ tokens per engagement on cloud models. Local LLMs avoid this entirely but trade off capability.

---

## Disclaimer

All tools listed are intended for **authorised penetration testing and security assessments only**.
Always ensure you have written permission before scanning any network or system.
The author accepts no responsibility for unauthorised or illegal use.

---

## Author

**gpheheise** — [github.com/gpheheise](https://github.com/gpheheise)
