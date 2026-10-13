# Platforma Scoala

Aplicație de desktop (Windows) pentru colegii din școală: un chat comun unde se
scriu mesaje și se atașează fișiere. Toți colegii văd același canal. Funcționează
pe mai multe calculatoare, în timp real, prin Firebase (gratuit).

## Ce poate acum (versiunea 1)
- Login cu e-mail și parolă (conturile sunt create de administrator).
- La prima intrare, fiecare își scrie numele afișat.
- Chat comun în timp real.
- Atașare de fișiere mici (până la 700 KB): poze, documente scurte, PDF-uri mici.
- Ștergerea propriilor mesaje; administratorii pot șterge orice mesaj.

Fișierele mari vor fi activate când se pornește stocarea extinsă (planul Blaze).

## Cum obții instalerul .exe (prin GitHub, fără Android Studio / unelte locale)
1. Urcă tot acest folder într-un depozit nou pe github.com.
2. Tab-ul **Actions** → workflow-ul „Construieste Windows” pornește singur.
3. După ~5 minute, deschide rularea → **Artifacts** → descarcă `PlatformaScoala-Windows`.
4. Dezarhivează și distribuie fișierul `.exe` colegilor. Îl deschid și instalează.

## Configurare (deja completată)
- `index.html` conține cheile proiectului Firebase și, în `ADMIN_EMAILS`,
  adresele administratorilor.
- `firestore.rules` conține regulile de securitate (de pus în consola Firebase).

## Dezvoltare locală (opțional)
```
npm install
npm start
```
