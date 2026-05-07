# Awesome AI Agent Security & Red Teaming Tools 🛡️🤖

A curated list of automated security tools for auditing AI agents, LLMs, and agentic workflows. This repository focuses on tools capable of detecting jailbreaks, prompt injections, and misconfigurations in autonomous systems.

---

## 🚀 Red Teaming & Jailbreak Scanners

### [Augustus (by Praetorian)](https://github.com/praetorian-inc/augustus)
* **What it does exceptionally well:** Automated adversarial scanning with over 210+ built-in attack vectors. It excels at identifying complex jailbreaks and encoding-based bypasses.
* **Why use it:** Best for high-coverage security audits where you need to stress-test a model against a massive library of known adversarial prompts.

### [Garak](https://github.com/leondz/garak)
* **What it does exceptionally well:** Acts as the "nmap for LLMs." It probes for hallucinations, data leakage, and injections using a modular approach.
* **Why use it:** Use this for initial reconnaissance and vulnerability discovery on any LLM-based interface.

### [PyRIT (by Microsoft)](https://github.com/Azure/pyrit)
* **What it does exceptionally well:** Orchestrating multi-stage attack chains. It allows researchers to use AI agents to attack other AI agents autonomously.
* **Why use it:** Perfect for researching "agentic" risks where a single prompt isn't enough, but a conversation is required to trigger a vulnerability.

---

## 🛠️ Pentesting & Vulnerability Research

### [PentestGPT](https://github.com/GreyDaze/PentestGPT)
* **What it does exceptionally well:** Providing a structured, AI-driven task tree for manual security engagements. It maintains state across complex exploitation phases.
* **Why use it:** Ideal for researchers who want an interactive partner during CTFs or live pentesting sessions on MacOS/Kali.

### [Promptfoo](https://github.com/promptfoo/promptfoo)
* **What it does exceptionally well:** CI/CD integrated testing. It allows you to run deterministic tests against agent outputs to ensure security patches actually work.
* **Why use it:** Use this for regression testing and ensuring that "system prompt" hardening remains effective after model updates.

### [PentAGI](https://github.com/microsoft/PentAGI)
* **What it does exceptionally well:** Autonomous multi-agent coordination within isolated Docker environments to find and exploit infrastructure flaws.
* **Why use it:** Best for experimental research into how AI can automate the full exploit lifecycle.

---

## ⚙️ Configuration & Posture Management

### [DefenseClaw (Cisco)](https://github.com/cisco-open/defenseclaw)
* **What it does exceptionally well:** Scanning agent "skills" and Model Context Protocol (MCP) integrations for excessive permissions.
* **Why use it:** Use this to check for "excessive agency"—situations where an agent has more access to your OS or APIs than it should.

### [Giskard](https://github.com/Giskard-AI/giskard)
* **What it does exceptionally well:** Detecting "performance-based" security flaws, such as bias, toxicity, and susceptibility to specific domain-driven injections.
* **Why use it:** Great for deep-dive Python-based analysis of model behavior and safety guardrails.

---

## 💻 Tech Stack Compatibility
* **MacOS (M1/M2/M3):** Most tools are Python-based and run natively.
* **Kali Linux / Windows VM:** Recommended for running autonomous agents like PentAGI or heavy network-based scanners to ensure environment isolation.

---

## ⚖️ Disclaimer

I am not responsible for any damage caused by the tools listed here. This list is for **educational and ethical security research purposes only**. Always ensure you have explicit permission before testing any system that is not your own.

---

## 🤝 Contribution
Found a new tool? Feel free to open a PR!

---

*Made by @gpheheise*
