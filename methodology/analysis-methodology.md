# Analysis Methodology

This document describes a cautious, reproducible workflow for authorized reverse-engineering research.

## 1. Authorization and scope

- Analyze only software you own, are authorized to inspect, or that is explicitly provided for research.
- Define the question before analysis: function behavior, file format, crash cause, or a specific indicator.
- Do not attempt unauthorized access, credential collection, evasion, or deployment of malware.

## 2. Preserve the sample

Record:
- Original filename and source
- Acquisition date and authorization context
- File size
- SHA-256 hash
- Whether the file is a source file, executable, archive, or extracted artifact

Keep an untouched copy. Do not rely on filenames alone to identify a sample.

## 3. Static triage

Using appropriate tools such as Ghidra, Cutter/radare2, and PE inspection utilities:
- Identify file format and architecture.
- Inspect headers, sections, imports, exports, and strings.
- Note suspicious or unusual features without treating them as proof.
- Select relevant functions and record addresses or symbols.
- Compare disassembly with decompiler output.
- Explain control flow and function behavior in your own words.

## 4. Dynamic analysis (only when necessary)

- Use a dedicated, isolated lab environment with snapshots and no personal accounts or sensitive files.
- Avoid running unknown samples on a daily-use computer.
- Use synthetic data and controlled network conditions.
- Record the exact sample hash, environment, timestamps, and observed actions.
- Distinguish observed behavior from inferred behavior.

## 5. Evidence and confidence

For every important claim, record:
- **Observation:** what was directly seen
- **Source:** file, function, line, address, log, or report
- **Interpretation:** what the observation may mean
- **Alternatives:** benign explanations or other possibilities
- **Confidence:** low, medium, or high, with a reason

Use terms such as “possible,” “consistent with,” or “not confirmed” when the evidence is incomplete.

## 6. Report structure

Each case report should include:
1. Title and status
2. Objective
3. Scope and authorization
4. Sample identity and hash
5. Tools and versions
6. Observations
7. Interpretation
8. Limitations
9. Conclusion
10. Reproducibility notes

## 7. Publication and privacy

- Do not upload binaries, payloads, private sandbox exports, credentials, tokens, or proprietary source code.
- Remove personal information from screenshots and logs.
- Do not claim that a file is malicious based only on a low-confidence score, suspicious filename, or isolated indicator.
- Clearly label reconstructed notes and unverified claims.

## 8. Reproducibility checklist

- [ ] The sample identity is unambiguous.
- [ ] Hashes were recalculated from the actual file.
- [ ] Tool versions and environment are recorded.
- [ ] Findings cite concrete evidence.
- [ ] Observations are separated from interpretation.
- [ ] Limitations and alternative explanations are included.
- [ ] Sensitive information is removed before publication.
