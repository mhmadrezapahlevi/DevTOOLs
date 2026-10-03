# DevTools

**Live demo:** https://mhmadrezapahlevi.github.io/DevTOOLs/

All tools run **100% in the browser** (client-side). There is no backend, and no data is sent to or stored on any server — the JSON, text, or code files you process never leave your device.

## List of Tools

| Tool | File | Features |
|---|---|---|
| 🧩 JSON Toolkit | `json-toolkit.html` | Format & validate JSON, minify, convert JSON→XML, JSON→CSV |
| 🔐 Encoder / Decoder | `encode-decode.html` | Base64, URL, HTML entity — two-way encode & decode |
| 🔑 UUID & Hash Generator | `uuid-hash.html` | Generate UUID v4 in bulk, compute MD5, SHA-1, SHA-256, SHA-384, SHA-512 |
| 🛠️ Code Formatter | `code-formatter.html` | Format XML, CSS, JavaScript, and SQL |
| 📝 Markdown & YAML | `markdown-yaml.html` | Markdown → HTML preview, YAML ↔ JSON conversion |
| 🔍 Diff Checker | `diff-checker.html` | Compare two texts or JSON line by line |
| ⏱️ Timestamp, Lorem & Regex | `timestamp-lorem-regex.html` | Convert Unix timestamp ↔ date, Lorem Ipsum generator, regex tester |

The main page (`index.html`) links to all the tools above.

## Running Locally

No installation is required — simply open any `.html` file directly in your browser:

```bash
git clone https://github.com/mhmadrezapahlevi/DevTOOLs.git
cd DevTOOLs
# open index.html in your browser, or run a local server:
python -m http.server 8000
```

Then go to `http://localhost:8000`.

## Technologies

Each tool is a standalone HTML file (vanilla JavaScript), with several open-source libraries loaded from a CDN for certain features:

- [marked.js](https://marked.js.org/) — Markdown rendering
- [js-yaml](https://github.com/nodeca/js-yaml) — YAML parsing/serialization
- [js-beautify](https://github.com/beautify-web/js-beautify) — CSS & JavaScript formatting

The rest (JSON handling, Base64/URL/HTML encoding, MD5, UUID, diff, SQL formatter, etc.) is written natively without dependencies, and the browser's Web Crypto API is used for SHA-1/256/384/512 hashing.

## License

MIT — see [LICENSE](LICENSE).
