# petrsimek.github.io

Rozcestník osobních projektů Petra Šimka, hostovaný jako GitHub user page.

## Účel

Jediný HTML soubor (`index.html`) sloužící jako landing page na `https://petrsimek.github.io/`. Odkazuje na jednotlivé project pages:

- `strazci` → `https://petrsimek.github.io/strazci/` (samostatný repozitář)

Každý projekt je hostovaný ve vlastním GitHub repozitáři jako project page. Tento rozcestník je společné rozhraní.

## Struktura

- `index.html` – kompletní rozcestník (HTML + inline CSS, žádný build)
- `CLAUDE.md` – tento soubor

Žádný `dist/`, žádný build skript. Vše se deployuje přímo.

## Design

- Roboto font z Google Fonts
- Čistý bílý background, modrý accent (`#1565c0`)
- Stejné CSS proměnné (`--radius`, `--ease` atd.) jako používá projekt `strazci` – pro vizuální konzistenci napříč projekty

## Deploy

Repozitář je veřejný GitHub repo s názvem přesně `petrsimek.github.io` (konvence GitHub Pages pro user page). Cokoli commitnutého do `main` je automaticky na `https://petrsimek.github.io/`.

```bash
git add -A && git commit -m "Update" && git push
```

## Přidání nového projektu

1. Nový projekt deployni jako samostatný repozitář s Pages (jako `strazci`)
2. Přidej kartu `<a class="project">` do sekce `.projects` v `index.html`
3. Commit + push

## Konvence

- Všechny externí odkazy otevírat do nového okna: `target="_blank" rel="noopener"`
- Interní linky na podcesty (`/strazci/`) zůstávají ve stejném okně
