# Versioning protocol

Status: proposed repository convention.

## Rules

- Use Git for the revision history of ordinary working files; keep their names stable.
- Write short, meaningful commit messages and commit coherent changes together.
- Use release tags such as `v1.0.0` only when a release is intentionally created. If using Semantic Versioning, first define the public interface or compatibility contract; do not claim SemVer compliance solely from a numeric pattern.
- Use explicit dates for time-indexed records and versioned names for externally distributed snapshots or immutable artifacts when needed.
- Never replace provenance with `final`, `final2`, or `latest` in filenames. A changelog or manifest can document release identity and lineage.
- Do not push, tag, or publish on behalf of the maintainer without authorization.

## Examples

| Resource | Convention |
| --- | --- |
| Working protocol | `file-naming.md` |
| Release tag | `v1.0.0` |
| Published archive | `engineering-dictionary__v1.0.0.zip` |
| Meeting record | `2026-11-26__meeting.md` |

See [file naming](file-naming.md).
