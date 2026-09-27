# DevTools

**Demo langsung:** https://mhmadrezapahlevi.github.io/DevTOOLs/

Semua tool berjalan **100% di browser** (client-side). Tidak ada backend, tidak ada data yang dikirim atau disimpan di server mana pun — file JSON, teks, atau kode yang Anda proses tidak pernah meninggalkan perangkat Anda.

## Daftar Tool

| Tool | File | Fitur |
|---|---|---|
| 🧩 JSON Toolkit | `json-toolkit.html` | Format & validasi JSON, minify, konversi JSON→XML, JSON→CSV |
| 🔐 Encoder / Decoder | `encode-decode.html` | Base64, URL, HTML entity — encode & decode dua arah |
| 🔑 UUID & Hash Generator | `uuid-hash.html` | Generate UUID v4 massal, hitung MD5, SHA-1, SHA-256, SHA-384, SHA-512 |
| 🛠️ Formatter Kode | `code-formatter.html` | Rapikan XML, CSS, JavaScript, dan SQL |
| 📝 Markdown & YAML | `markdown-yaml.html` | Pratinjau Markdown → HTML, konversi YAML ↔ JSON |
| 🔍 Diff Checker | `diff-checker.html` | Bandingkan dua teks atau JSON baris demi baris |
| ⏱️ Timestamp, Lorem & Regex | `timestamp-lorem-regex.html` | Konversi Unix timestamp ↔ tanggal, generator Lorem Ipsum, penguji regex |

Halaman utama (`index.html`) menautkan ke semua tool di atas.

## Menjalankan secara lokal

Tidak perlu instalasi apa pun — cukup buka salah satu file `.html` langsung di browser:

```bash
git clone https://github.com/mhmadrezapahlevi/DevTOOLs.git
cd DevTOOLs
# buka index.html di browser, atau jalankan local server:
python -m http.server 8000
```

Lalu akses `http://localhost:8000`.

## Teknologi

Setiap tool adalah file HTML mandiri (vanilla JavaScript), dengan beberapa library open-source yang dimuat dari CDN untuk fitur tertentu:

- [marked.js](https://marked.js.org/) — rendering Markdown
- [js-yaml](https://github.com/nodeca/js-yaml) — parsing/serialisasi YAML
- [js-beautify](https://github.com/beautify-web/js-beautify) — format CSS & JavaScript

Sisanya (JSON handling, Base64/URL/HTML encoding, MD5, UUID, diff, SQL formatter, dll) ditulis native tanpa dependency, dan Web Crypto API browser dipakai untuk hash SHA-1/256/384/512.

## Lisensi

MIT — lihat [LICENSE](LICENSE).
