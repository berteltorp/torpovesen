# Torp Ovesen ApS — website

Simpel statisk one-page site for **Torp Ovesen ApS**, et privat holdingselskab,
i ren HTML/CSS. Ingen byggeproces og ingen eksterne afhængigheder — filerne
serveres som de er.

> Navnet "Torp Ovesen ApS" hører til det juridiske selskab med CVR **37904139**
> (pt. registreret som *Bertel Torp Holding ApS*). Se "Navneændring i CVR" nedenfor.

## Filer

- `index.html` — hele siden (én side)
- `style.css` — moderne minimal styling
- `favicon.svg` — "TO"-monogram
- `.nojekyll` — fortæller GitHub Pages, at filerne skal serveres råt

## Se siden lokalt

```sh
open index.html
# eller, tættest på GitHub Pages:
python3 -m http.server 8000   # besøg http://localhost:8000
```

## Udgiv på GitHub Pages

1. Opret et repo og push denne mappe:

   ```sh
   git init
   git add .
   git commit -m "Torp Ovesen site"
   git branch -M main
   git remote add origin https://github.com/<bruger>/torpovesen.git
   git push -u origin main
   ```

2. På GitHub: **Settings → Pages → Source: `main` / `/ (root)`** og gem.
3. Siden går live på `https://<bruger>.github.io/torpovesen/` (kan tage et par minutter).

## Eget domæne (torpovesen.com)

1. Registrér `torpovesen.com` hos en registrar.
2. Tilføj en fil `CNAME` i denne mappe med kun domænet:

   ```
   torpovesen.com
   ```

3. Opret DNS (A-records til GitHub Pages' IP'er eller CNAME til `<bruger>.github.io`).
4. Aktivér under **Settings → Pages → Custom domain**.

## Navneændring i CVR (udføres på virk.dk)

Selve selskabsnavnet ændres uafhængigt af denne side:

1. Tjek at det ønskede navn (fx "Torp Ovesen ApS") er ledigt i CVR-registret.
2. Ejer vedtager vedtægtsændring (navn) og protokollerer beslutningen.
3. Registrér det nye navn hos Erhvervsstyrelsen på virk.dk (typisk gebyrfrit).
4. CVR-nummeret **37904139 forbliver det samme** — ejerbog-linket på siden gælder fortsat.
5. Opdater footer/legal-tekst på siden, når ændringen er registreret.
