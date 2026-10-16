# Reverse Engineering Portfolio

A student portfolio documenting software reverse-engineering practice with Ghidra, Cutter, and radare2.

## Scope

This repository focuses on:
- Static inspection of compiled programs
- Assembly and decompiled-function explanation
- Recording observable indicators without overstating conclusions
- Safe, authorized analysis and reproducible notes

## Important evidence note

Some case files in this repository were reconstructed from prior notes and summaries, not from the original binaries or complete sandbox exports. They are marked **preliminary** where source evidence is incomplete. Hashes, detections, and behavior claims should be verified against the original artifacts before being treated as confirmed findings.

## Case files

| File | Topic | Status |
|---|---|---|
| `cases/01-cli-zen-analysis.md` | `cli.exe` / `zen.exe` investigation notes | Preliminary; verify hash and artifacts |
| `cases/02-dismhost-artifacts.md` | Two `DISMHOST.EXE`-named artifacts | Preliminary; relationship not established |
| `cases/03-obfuscated-lua-analysis.md` | Obfuscated Lua-like code and loader flow | Preliminary; full source unavailable |
| `cases/04-possible-stealer-indicators.md` | Possible information-stealing behavior | Hypothesis; requires direct evidence |
| `cases/05-calipso-incomplete.md` | `Calipso.exe` metadata lead | Incomplete |
| `cases/06-edgev5-pending.md` | `Edgev5.exe` research lead | Pending source evidence |

## Methodology

See [`methodology/analysis-methodology.md`](methodology/analysis-methodology.md) for a repeatable workflow and reporting standards.

## Safety and authorization

Only analyze software you own, have explicit permission to inspect, or that is provided for legitimate research. Do not publish malware samples, credentials, tokens, private sandbox data, or proprietary code. Do not execute unknown samples on a daily-use machine. A suspicious indicator alone is not proof of maliciousness.

## Contact

Add a professional contact method here only when you are ready to receive legitimate inquiries.
