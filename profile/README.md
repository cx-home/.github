<p align="center"><img src="cx-logo.png" width="96" alt="cx"></p>

# cx

CX is one bracketed syntax for documents, queries, programs and the compiler's
own tree — exact decimals, deny-by-default effects, errors as values, a
content-addressed store. If you've ever needed a data format, a query
language and a general-purpose language to agree with each other, this is
what that agreement looks like: one grammar, everywhere.

**Start here:** [cxhome.org](https://cxhome.org) — the primer, the guide, the
full reference (rendered from every repository below, at the pin), and the
install. Everything narrative lives on that one site (RULED: D57a, D58a); this
page is a pointer, not a copy.

## The repositories

| group | repository | what it is | ships |
|---|---|---|---|
| the front door | [cx](https://github.com/cx-home/cx) | the front door: pins every repo, builds the four cx builds and libcx-core/libcx, holds the site, the release, the installer | binary |
| the two cores | [cx-core-data](https://github.com/cx-home/cx-core-data) | the data format: reader, writer, canonical form, schema, codecs, libcx-core, the data-only cx | binary |
|  | [cx-core-code](https://github.com/cx-home/cx-core-code) | the language: evaluator, stdlib, LSP, libcx, the cli and embed builds | binary |
| the platform group | [cx-platform-net](https://github.com/cx-home/cx-platform-net) | sockets, TLS, the HTTP server, the XSP transport bindings, ftp, sftp, file_surface | binary |
|  | [cx-platform-mail](https://github.com/cx-home/cx-platform-mail) | SMTP and IMAP, server and client cores, sasl | binary |
|  | [cx-platform-identity](https://github.com/cx-home/cx-platform-identity) | sessions, did:web, authz-store, vc-revocation | binary |
|  | [cx-platform-store](https://github.com/cx-home/cx-platform-store) | the storage engine, its substrates, journal/live/audit, ft, and the store server | binary |
|  | [cx-platform-db](https://github.com/cx-home/cx-platform-db) | external database access: $sql-*, $redis-*, the drivers | binary |
|  | [cx-platform-fabric](https://github.com/cx-home/cx-platform-fabric) | messaging and fabric-serve | binary |
|  | [cx-platform-xsp](https://github.com/cx-home/cx-platform-xsp) | the XAP Stream Protocol: the frame codec, the XSP-AUTH handshake, the protocol pages | binary |
|  | [cx-platform-xap](https://github.com/cx-home/cx-platform-xap) | the application host, compose, dist, schema, market, the reference deployments | binary |
|  | [cx-platform-flow](https://github.com/cx-home/cx-platform-flow) | workflow; its CLI verbs stay in the binary | package |
|  | [cx-platform-connector](https://github.com/cx-home/cx-platform-connector) | the connector kit and sync | package |
|  | [cx-platform-secrets](https://github.com/cx-home/cx-platform-secrets) | the minimal keystore: one handle grammar, one internal resolve seam, the PEP and the audit record, custody that rises by a provider row | package |
|  | [cx-platform-sso](https://github.com/cx-home/cx-platform-sso) | enterprise sign-on, the interop lane | package |
|  | [cx-platform-ux](https://github.com/cx-home/cx-platform-ux) | the web and terminal surfaces | package |
|  | [cx-platform-agent](https://github.com/cx-home/cx-platform-agent) | tools, mcp, mcp-server, a2a, a2a-xap, llm, run, adjudicate | package |
| the bindings | [cx-binding-python](https://github.com/cx-home/cx-binding-python) | cxlib for Python | pypi |
|  | [cx-binding-go](https://github.com/cx-home/cx-binding-go) | cxlib for Go | go-module |
|  | [cx-binding-rust](https://github.com/cx-home/cx-binding-rust) | cxlib for Rust | crate |
|  | [cx-binding-v](https://github.com/cx-home/cx-binding-v) | the native reference binding | v-module |
| the ecosystem | [cx-registry](https://github.com/cx-home/cx-registry) | the package index: the store, publisher keys, the publish program | none |
|  | [cx-decisions](https://github.com/cx-home/cx-decisions) | the ledger, the process specs, the standing rules, design texts | none |
|  | [cx-tooling](https://github.com/cx-home/cx-tooling) | vscode, neovim, tree-sitter, completions, syntax, the installer, diagram | editor |

Each repository below is thin by design (RULED: D58a): a README, a
CONTRIBUTING, and its generated reference fragment — the narrative is on
[cxhome.org](https://cxhome.org), which indexes every fragment as it is
published. `cx` is the front door: it pins every repository above, builds the
four `cx` builds, and holds the release, the installer and the site.

## Contributing

Each repository carries its own `CONTRIBUTING.md`. Cross-cutting decisions
live in [`cx-decisions`](https://github.com/cx-home/cx-decisions); the
path→repository allocation and the module registry live in
[`cx-registry`](https://github.com/cx-home/cx-registry).
