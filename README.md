# BT-EPP-auta — PR-278 Neživot Auta

Statický prototyp pojišťovacího wizardu (single-file HTML). Hlavní soubor je [`index.html`](./index.html).

## Lokální spuštění

Stačí otevřít `index.html` v prohlížeči. Nebo lokální server:

```bash
python3 -m http.server 8000
# → http://localhost:8000
```

## Struktura

| Soubor | Popis |
| --- | --- |
| `index.html` | Celý prototyp (HTML + CSS + JS v jednom souboru) |
| `vercel.json` | Konfigurace nasazení (clean URLs) |
| `.gitignore` | Ignorované soubory |

## Nasazení na Vercel

1. Vytvoř repozitář na GitHubu a nahraj tento projekt:
   ```bash
   git remote add origin https://github.com/<uživatel>/BT-EPP-auta.git
   git push -u origin main
   ```
2. Na [vercel.com](https://vercel.com) → **Add New… → Project** → importuj repozitář.
3. Framework Preset: **Other** (statický web), Build Command: prázdné, Output Directory: prázdné — Vercel servíruje `index.html` z rootu.
4. **Deploy.** Každý další `git push` do `main` nasadí novou verzi automaticky.

## Další úpravy

Prototyp je jeden soubor — uprav `index.html`, commitni a pushni. Změny se projeví na Vercelu po nasazení.
