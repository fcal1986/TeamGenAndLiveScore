# Spielr 🎲

Teams auslosen, Turniere starten, fair entscheiden.  
Login via **Google OAuth** oder **Magic Link**.

## Setup (einmalig)

### 1. Supabase SQL ausführen
→ Supabase Dashboard → SQL Editor → `supabase_setup.sql` einfügen → Run

### 2. Google OAuth in Supabase aktivieren
→ Authentication → Providers → Google → Enable  
→ Client ID + Secret aus Google Cloud Console eintragen  
→ Redirect URL kopieren (wird von Supabase angezeigt) → in Google Cloud eintragen

### 3. Supabase Site URL setzen
→ Authentication → URL Configuration  
→ Site URL: `https://[dein-username].github.io/spielr/`  
→ Redirect URLs hinzufügen: `https://[dein-username].github.io/spielr/index.html`

### 4. GitHub Secrets setzen
→ Repository → Settings → Secrets and variables → Actions  
→ `SUPABASE_URL` = `https://djhxhkhcuvuyozyqmnew.supabase.co`  
→ `SUPABASE_ANON_KEY` = dein Publishable API Key

### 5. GitHub Pages aktivieren
→ Repository → Settings → Pages  
→ Source: **GitHub Actions**

Jeder Push auf `main` deployt automatisch. ~1 Minute bis live.
