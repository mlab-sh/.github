<div align="center">

# 🧪 MLAB

**Investigate threats, not noise.**

The complete cyber platform - IOC & file intelligence, incident response,
threat hunting and third-party risk, unified in one ecosystem.
Built for SOC teams, DFIR and threat researchers who need signal, not noise.

[🌐 mlab.sh](https://mlab.sh) · [🧭 Ecosystem](https://mlab.sh/ecosystem) · [📖 Docs](https://doc.mlab.sh/docs/mlab.sh) · [🧰 Free tools](https://mlab.sh/tools) · [𝕏 @Sn0wAlice](https://x.com/Sn0wAlice)

</div>

---

## 🔎 Core - [mlab.sh](https://mlab.sh)

IOC & file intelligence. Drop in an IP, a domain, a hash, a certificate or a file
and get back structured, actionable context - not a page of results to triage.

```console
$ mlab scan domain sso-login-verify.example

  DNS         A 203.0.113.47 · AAAA 2001:db8::47 · no CNAME
  Email       SPF ~all · DKIM sig1 · DMARC missing
  TLS         Let's Encrypt · valid to 2026-10-24 · 2 issuers seen
  Subdomains  4 found - mail, vpn, sso-portal · 1 flagged suspicious
  Files       no security.txt · robots.txt disallows /admin
```

Files go through static and dynamic analysis (EXE, DLL, PDF, Office…), infrastructure
gets correlated, findings get mapped to MITRE ATT&CK. All of it available through the
[REST API](https://doc.mlab.sh/docs/mlab.sh), [MCP](https://doc.mlab.sh/docs/mlab.sh/integrations/mcp)
and the [CLI](https://github.com/mlab-sh/mlab-cli).

---

## 🧰 Open source

Rust-first, built in the open. Single static binaries, no daemon, no telemetry.

| Project | What it does |
| ------- | ------------ |
| **[postmortem](https://github.com/mlab-sh/postmortem)** | Supply-chain scanner. Flags malicious install code, typosquats and shady provenance across your dependencies *and* your OS packages. Repo-reputation scoring, known-CVE intel. Node, Python, Rust, Ruby, PHP, Go, JVM |
| **[assay](https://github.com/mlab-sh/assay)** | Offline-first scanner for ML model artifacts - safetensors, GGUF, PyTorch pickle. Know what you just downloaded before you load it |
| **[mcpwn](https://github.com/mlab-sh/mcpwn)** | Static security scanner for MCP servers. 36 rules over tool definitions - shadowed names, rug pulls, toxic data flows, dangerous capabilities. SARIF out |
| **[k3sec](https://github.com/mlab-sh/k3sec)** | Runtime security CLI for k3s clusters. eBPF syscall tracing and YARA detections merged into one live event stream |

**Infra auditors** - point them at an API, get graded findings back. Read-only (every request is a GET), snapshot & diff, CVEs matched to the exact installed version.

| Project | Audits |
| ------- | ------ |
| **[mlab-cloudflare](https://github.com/mlab-sh/mlab-cloudflare)** | Cloudflare account - DNS, edge posture, TLS, Workers, Zero Trust, logging, IAM. One exit code for CI |
| **[mlab-scw](https://github.com/mlab-sh/mlab-scw)** | Scaleway account - IAM weaknesses, internet exposure, plaintext credentials, published CVEs |
| **[mlab-proxmox](https://github.com/mlab-sh/mlab-proxmox)** | Proxmox VE cluster - access control, firewall, guest isolation, backups, patch level |
| **[mlab-unifi](https://github.com/mlab-sh/mlab-unifi)** | UniFi console - segmentation, firewall, Wi-Fi, exposure |
| **[mlab-mikrotik](https://github.com/mlab-sh/mlab-mikrotik)** | MikroTik RouterOS - exposure, firewall, accounts |

---

## 🔌 Integrations

Plug mlab.sh into the tools you already use.

**SOC stack** - enrich alerts with hash, URL, IP and CVE intel (KEV, EPSS, Tor), hand incidents to [ir.mlab.sh](https://ir.mlab.sh/overview).

| Integration | What it does |
| ----------- | ------------ |
| **[mlab-splunk](https://github.com/mlab-sh/mlab-splunk)** | Splunk app - `\| mlab` search command, adaptive response for Enterprise Security |
| **[mlab-wazuh](https://github.com/mlab-sh/mlab-wazuh)** | Drop-in integratord scripts and rules, no dependencies |
| **[shuffle-node](https://github.com/mlab-sh/shuffle-node)** | Shuffle SOAR app - IOC scanning & extraction, CVE and threat-actor data |
| **[n8n-nodes-mlab](https://github.com/mlab-sh/n8n-nodes-mlab)** | Verified n8n community node - drop IOC enrichment into any workflow |
| **[mlab-glpi](https://github.com/mlab-sh/mlab-glpi)** | GLPI 11 plugin - matches your inventory's installed software against CVEs, prioritises by KEV/EPSS/CVSS, opens tickets |

**Dev & agents**

| Integration | What it does |
| ----------- | ------------ |
| **[mlab-cli](https://github.com/mlab-sh/mlab-cli)** | Scan domains, IPs, files and URLs, extract IOCs, search CVEs and threat actors, gate CI on vulnerable dependencies. Terminal or JSON |
| **[VS Code](https://marketplace.visualstudio.com/items?itemName=mlab-sh.vuln-scan)** · **[JetBrains](https://github.com/mlab-sh/vuln-scan-jetbrains)** | CVE scanning for your lockfiles (npm, Cargo, Go, Composer, Ruby, Python), prioritised with EPSS and CISA/EU KEV |
| **[MCP server](https://doc.mlab.sh/docs/mlab.sh/integrations/mcp)** | Give Claude, Cursor or any MCP client direct access to mlab.sh - scan IOCs and pull intel from inside your agent |
| **[Claude Code plugin](https://github.com/mlab-sh/mlab-claude)** | Ready-made SOC/DFIR and supply-chain skills - IOC triage, phishing, dependency review, SBOM audit |
| **[nav-ext](https://github.com/mlab-sh/nav-ext)** | Chrome & Firefox extension. Highlights domain and IP IOCs on any page, pivot to an investigation in one click |

---

## 🧭 The ecosystem

> Security is not a product. It's a practice.

35 modules across governance, detection, attack surface, deception & endpoint and training.
One data model, one API surface, one alerting pipeline. No silos, no gaps, no noise.

**→ [mlab.sh/ecosystem](https://mlab.sh/ecosystem)** - the full, always up-to-date list.

---

## 🤝 Get involved

- **Bug reports / PRs** → always welcome
- **Questions** → open an issue or ping [@Sn0wAlice](https://x.com/Sn0wAlice)

---

<div align="center">

_Mlab · by Cyber Dream_ 🏴

</div>
