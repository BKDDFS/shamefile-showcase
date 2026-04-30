# Contributing to shamefile-showcase

This repository collects real-world `shamefile.yaml` examples generated
from popular open-source projects. Each entry demonstrates shamefile
running on a real codebase in a supported language.

## What lives here

No source code — only `shamefile.yaml` files and metadata. The upstream
project URL and commit SHA are recorded so anyone can reproduce the scan
or browse the original code.

Directory structure:

```
<language>/<project>/
├── shamefile.yaml
└── README.md
```

The `README.md` per entry must contain:

- Upstream project URL
- Commit SHA used for the scan
- Suppression count
- Link to the shamefile issue that tracks this language
- Whether AI assistance was used to fill `why` fields

## How to contribute

Open an issue in the main
[shamefile](https://github.com/BKDDFS/shamefile) repository using the
**Verify and release a language** template. That issue walks you through
the full process — generating `shamefile.yaml` against an upstream
project, filling `why` fields, and opening a PR here.

Do not open a PR here without a corresponding issue in the main repo.

## Review scope

Maintainers review `shamefile.yaml` entries and the metadata README.
Source code of the upstream project is not reviewed — it is a
vendored artifact at a pinned commit SHA, verifiable against the
upstream repository.

## License

Entries in this repository are released under
[Apache 2.0](LICENSE). Upstream project source code is not included;
`shamefile.yaml` contains only metadata (file paths, token names,
suppression counts, and written justifications) and does not
constitute a copy of the upstream work.
