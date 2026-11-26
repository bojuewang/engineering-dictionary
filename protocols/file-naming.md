# File naming protocol

Status: proposed repository convention (UFNP — Universal File Naming Protocol). This name is local, not an assertion of international standardization.

## Scope

Repository-owned filenames, including documentation, data, and research artifacts. Required tool conventions and third-party filenames are exceptions.

## Rules

1. Ordinary names use lowercase ASCII letters, digits, and hyphens; use `__` between distinct semantic fields only when useful.
2. Use the shortest name that is unambiguous within its directory. Do not repeat information already provided by its path.
3. Prefer the optional semantic pattern `subject__type__qualifier.ext`; omit fields not needed for identification. Field semantics are contextual; use structured metadata if they must be parsed unambiguously.
4. Use the actual lowercase format extension for repository-owned files. Compound extensions (e.g. `.tar.gz`) and extensionless files are permitted where appropriate.
5. For dated records use `YYYY-MM-DD` and for fixed-width identifiers use an agreed width, e.g. `001`. Use version identifiers in names only when distributing versioned or immutable artifacts; see [versioning](versioning.md).
6. Avoid spaces, control characters, Windows-reserved characters and device names, trailing dots/spaces, and case-only distinctions. Keep paths reasonably short.
7. Existing ecosystem conventions take precedence: e.g. `README.md`, `AGENTS.md`, `LICENSE`, `.gitignore`, and Python module `snake_case`. Never rename an externally required filename just for cosmetic uniformity.

A practical lexical pattern for ordinary, non-hidden names (not a complete portability validator):

```regex
^[a-z0-9]+(?:-[a-z0-9]+)*(?:__[a-z0-9]+(?:-[a-z0-9]+)*)*(?:\.[a-z0-9]+(?:-[a-z0-9]+)*)*$
```

The expression does not check calendar validity, Windows device names, file contents, or semantic field roles. Check those separately.

## Examples

| Preferred | Avoid | Reason |
| --- | --- | --- |
| `coefficient-matrix.json` | `Coefficient Matrix FINAL.json` | Stable and portable |
| `fpp__equations__bicanonical.json` | `data1.json` | Meaningful semantic fields |
| `2026-11-26__meeting.md` | `11-26-26 notes.md` | Unambiguous sortable date |
| `experiment-001.json` | `experiment 1.json` | Stable identifier and sorting |
| `README.md` | `readme-file-v2.md` | Established tool convention |

Within `fake-projective-planes/cs-a2-024/`, prefer `equations.json` to `fake-projective-plane-cs-a2-024__equations.json`.

## Verification

Check lexical consistency, reserved names, case collisions, semantic uniqueness, and ecosystem exceptions before renaming files. For existing paths, preserve compatibility or update references explicitly. No automatic rename is authorized by this protocol.
