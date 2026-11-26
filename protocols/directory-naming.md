# Directory naming protocol

Status: proposed repository convention.

## Rules

- Use lowercase `kebab-case` for ordinary directories; use names that describe a coherent namespace, responsibility, or object collection.
- Prefer short, meaningful paths and avoid duplicating ancestor names in descendants.
- Use plural collection names when appropriate (`protocols`, `templates`); established conventions such as `src` and `data` are allowed.
- Create directories when they contain meaningful resources. Avoid empty speculative branches.
- Respect external tool requirements (for example `.github`, `.git`, or importable Python package naming).

## Example

```text
research-project/
  data/
    raw/
    processed/
  experiments/
    experiment-001/
      configuration.json
      results.json
```

The directory path identifies the namespace; the file name identifies the local resource. See [file naming](file-naming.md).
