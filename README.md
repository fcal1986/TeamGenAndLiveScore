# Spielr 🎲

Teams auslosen, Turniere starten, fair entscheiden.

## GitHub Secrets einrichten

Damit der Deploy-Workflow die Supabase-Keys einsetzen kann:

1. GitHub Repository → **Settings** → **Secrets and variables** → **Actions**
2. **New repository secret** → Name: `SUPABASE_URL` → Value: deine Supabase Project URL
3. **New repository secret** → Name: `SUPABASE_ANON_KEY` → Value: dein Publishable API Key

## Supabase einrichten

SQL aus `supabase_setup.sql` einmalig im Supabase SQL Editor ausführen.

## Deploy

Jeder Push auf `main` deployt automatisch auf GitHub Pages.

Manuelle Auslösung: **Actions** → **Deploy Spielr to GitHub Pages** → **Run workflow**
