# General-Auditor

[General-Auditor](https://github.com/Unka-Malloc/General-Auditor) is the shared audit source for SymPolicy, Meshrix-Platform and LicoLand.
Each repository event applies common policy and that repository's profile only.
The workflow uses `Unka-Malloc/General-Auditor@only` and retains existing required audit status contexts.

Privacy, license, dependency, repository-policy and evidence findings are reviewed
in context by a contributor's local Agent. Hardcoded keyword matches are warnings,
not automatic leakage judgments. CI does not invoke a paid Agent service.

Local staged, working-tree, outgoing-range and reachable-history scans use the
[maintained initialization instructions](https://github.com/Unka-Malloc/General-Auditor/blob/only/docs/initialization.md).
Use the current `only` branch for the maintained CLI contract.
Reports retain exact source-match values and context only in ignored repository-local `.general-auditor/local/` files. Never publish or upload them.

CI checks do not generate reports or upload source evidence. Local scans create a self-contained HTML report in `.general-auditor/local/`; local contextual review determines whether a candidate is a real issue or false positive.
Auditor changes require a maintainer's temporary-branch PR to `only`.

- [Audit, License, and Dependency Compliance](../standards/audit-license-and-dependency-policy.md)
- [Repository Matrix and Source Priority](repository-matrix.md)
