# PUSHER static site

Open via a local HTTP server, not by double-clicking `index.html`, because browsers block `fetch()` from `file://` URLs.

```bash
cd pusher_site
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

Pages:
- `index.html` — homepage
- `index.html?lang=cs` — Czech
- `page.html?p=privacy&lang=en`
- `page.html?p=privacy&lang=cs`
- `page.html?p=terms&lang=en`
- `page.html?p=terms&lang=cs`

Supported languages: `en`, `cs`.

Files:
- `logo.png` — app icon (110×110, rounded corners via CSS)
- `content/privacy_en.md` / `privacy_cs.md` — Privacy Policy
- `content/terms_en.md` / `terms_cs.md` — Terms & Conditions
