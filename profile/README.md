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

---

## 🔌 Integrations

Plug mlab.sh into the tools you already use.

| Integration | What it does |
| ----------- | ------------ |
| **[mlab-cli](https://github.com/mlab-sh/mlab-cli)** | Official command-line client for mlab.sh and the CVE API at vuln.mlab.sh |
| **[n8n-nodes-mlab](https://github.com/mlab-sh/n8n-nodes-mlab)** | Verified n8n community node - drop IOC enrichment into any workflow |
| **[nav-ext](https://github.com/mlab-sh/nav-ext)** | Chrome & Firefox extension. Highlights domain and IP IOCs on any page, pivot to an investigation in one click |
| **[VS Code](https://marketplace.visualstudio.com/items?itemName=mlab-sh.vuln-scan)** | CVE scanning for your lockfiles, prioritised with EPSS and CISA KEV. Rescans on change, nothing leaves your machine until you agree |
| **[MCP server](https://doc.mlab.sh/docs/mlab.sh/integrations/mcp)** | Give Claude, Cursor or any MCP client direct access to mlab.sh - scan IOCs and pull intel from inside your agent |

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
