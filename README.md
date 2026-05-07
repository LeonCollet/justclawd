# JustClose · Clowdex-Style Preview

Dedizierte Preview-Site für die JustClose Sales-Betriebssystem-Landingpage (Clowdex-Layout, JustClose-Design).
Komplett unabhängig von der Hauptseite (Magic-UI Hero), eigener Deploy, eigene Domain.

## Inhalt
- `index.html` — die Landingpage (single-file, Inter + JetBrains Mono via Google Fonts, kein Build-Step)
- `logos/` — 11 Kunden-Logos
- `vercel.json` — Vercel-Config (clean URLs)

## Lokal ansehen
Doppelklick auf `index.html` öffnet sie direkt im Browser.

## Deploy auf Vercel

1. **Neues GitHub-Repo anlegen** (privat empfohlen):
   https://github.com/new → Name z.B. `justclose-clowdex-preview`
2. Diesen Ordner (`clowdex-preview/`) als Inhalt des Repos pushen — entweder via GitHub Desktop (clone das leere Repo, alle Files reinkopieren, commit, push) oder via Browser Drag-and-Drop ("Add file → Upload files").
3. **Vercel mit dem neuen Repo verbinden:**
   - Vercel Dashboard → "Add New… → Project"
   - GitHub-Repo auswählen
   - Application Preset: **Other**
   - Root Directory: `./` (Standard)
   - Build & Output Settings: leer lassen (ist eine statische Site)
   - Deploy
4. Nach 30-60 Sekunden ist die Preview live unter z.B. `justclose-clowdex-preview.vercel.app`.

## Custom Domain (optional)
In Vercel → Project → Settings → Domains → Custom Domain hinzufügen.
Bei externem Registrar: CNAME auf `cname.vercel-dns.com` setzen.

## Updates
Lokale Änderungen → commit → push. Vercel deployt automatisch.
