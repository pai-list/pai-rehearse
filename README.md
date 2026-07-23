<!-- ═══════════ PAI-REHEARSE · Cognitive Pre-Simulation ═══════════ -->
<!-- Stack: Python, multi-agent simulation, SAAM engine      -->
<!-- Includes: PAPER.md, 5 benchmarks, 4 persona system      -->
<!-- Updated: 23 July 2026                                   -->
<!-- ════════════════════════════════════════════════════════ -->

<div align="center">
  <img src="https://img.shields.io/badge/status-active-00FF41?style=flat-square&labelColor=0D1117" />
  <img src="https://img.shields.io/github/license/pai-list/pai-rehearse?style=flat-square&color=00A36C&labelColor=0D1117" />
  <img src="https://img.shields.io/badge/Python-3.12-3776AB?style=flat-square&logo=python&labelColor=0D1117" />
  <a href="PAPER.md"><img src="https://img.shields.io/badge/paper-PDF-FF6B6B?style=flat-square&labelColor=0D1117" /></a>
</div>

# ۞ PAI-Rehearse

**4-Persona Cognitive Pre-Simulation Protocol for SAAM-Al-Mizan — Mental Rehearsal & Self-Play Engine for Agents.**

PAI-Rehearse runs agents through a 4-persona cognitive simulation before deployment, identifying failure modes, trust boundaries, and capability gaps. Built on the SAAM-Al-Mizan framework for tri-regional model arbitration.

---

## ❯ The 4 Personas

| Persona | Role | Simulates |
|:--------|:-----|:----------|
| 🧠 **The Architect** | System designer | Protocol correctness, topology |
| ⚖️ **The Arbiter** | Trust & safety | Ethical boundaries, refusal gates |
| 🚀 **The Operator** | End-user | Usability, real-world edge cases |
| 🔬 **The Auditor** | Third-party | Security, verification, replay |

---

## ❯ Benchmarks

| Script | Purpose |
|:-------|:--------|
| `benchmarks/run_7_initializers_benchmark.py` | 7-pool initialization timing |
| `benchmarks/run_benchmark.py` | Core simulation throughput |
| `benchmarks/run_cross_language_benchmark.py` | Multi-language agent interop |
| `benchmarks/run_number_topology_benchmark.py` | Numeric topology validation |
| `benchmarks/run_tri_regional_benchmark.py` | US/CN/MENA routing accuracy |

---

## ❯ Quick Start

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt

# Run a rehearsal
python src/rehearse_engine.py --config pai-saam.jsonc

# Run benchmarks
python benchmarks/run_tri_regional_benchmark.py
```

---

## ❯ Output

A rehearsal produces a **Readiness Report**:

```
PAI-REHEARSE READINESS REPORT
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Architect:  ✅ 97.2%
Arbiter:    ✅ 94.8%
Operator:   ✅ 91.5%
Auditor:    ✅ 96.1%
────────────────────────────
OVERALL:    94.9% — DEPLOYMENT RECOMMENDED
```

---

## ❯ Research Paper

See [`PAPER.md`](PAPER.md) for the full theoretical framework.

---

## ❯ Related

- [`pai-list/pai-cli`](https://github.com/pai-list/pai-cli) — `pai rehearse` command
- [`pai-list/pai-agent-kit`](https://github.com/pai-list/pai-agent-kit) — Agent runtime
- [`pai-list/pai-mcp`](https://github.com/pai-list/pai-mcp) — MCP gateway

---

## ❯ License

MIT © [PAI Ecosystem](https://github.com/pai-list)

---

*Simulate before you deploy. Rehearse before you launch.*
