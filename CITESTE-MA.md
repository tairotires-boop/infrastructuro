# InfraHub — update major, septembrie 2026

## Continut

- `index.html` — pagina principala reconstruita (date la 6 septembrie 2026)
- 32 de directoare, fiecare cu propriul `index.html` (URL curat: /nume-pagina/)
- `assets/infrahub.css` — foaia de stil comuna
- `sitemap.xml`, `robots.txt`, `llms.txt`, `llms-full.txt`
- `_headers`, `_redirects`, `netlify.toml` — configurare Netlify

## Publicare pe Netlify — varianta rapida (drag & drop)

1. Dezarhiveaza pachetul. Rezulta directorul `infrahub-2026`.
2. Intra in contul Netlify si deschide site-ul EXISTENT (cel pe care e legat
   domeniul infrahub.ro). Nu crea site nou — ai pierde domeniul.
3. Tab-ul `Deploys` → zona "Drag and drop your site output folder here".
4. Trage directorul `infrahub-2026` (directorul intreg, nu continutul lui).
5. Astepti ~30 secunde. Deploy-ul apare in lista cu "Published".

Daca ceva e gresit, in lista de deploy-uri alegi versiunea anterioara →
`Publish deploy`. Revenirea e instantanee.

## Publicare prin Netlify CLI (optional)

    npm install -g netlify-cli
    netlify login
    cd infrahub-2026
    netlify link          # alegi site-ul existent
    netlify deploy --dir=. --prod

## Verificari dupa publicare

1. Deschide https://www.infrahub.ro/ si https://www.infrahub.ro/a7-autostrada-moldovei-2026/
2. Domeniul principal in Netlify (Domain management → Primary domain) trebuie sa fie
   `www.infrahub.ro`, pentru ca toate etichetele canonical din pagini indica www.
3. Google Search Console → Sitemaps → trimite `sitemap.xml`
4. Verifica datele structurate pe search.google.com/test/rich-results

## Cifre folosite in continut (verificate la 6 septembrie 2026)

- 1.476 km autostrada si drum expres deschisi circulatiei
- 12,24 km A3 Zimbor–Poarta Salajului (11 august 2026)
- 47,1 km A7 Adjud–Bacau Sud (31 august 2026)
- estimare 2026: circa 243 km
- PNRR incheiat 31 august 2026, buget final 20,1 mld euro, tinta rutiera 257 km (de la 429)
- SAFE: 16,68 mld euro alocare Romania, circa 4,2 mld euro la Transporturi
- siguranta rutiera: 68 decese/milion locuitori (2025 preliminar), media UE 43

Cand se schimba, actualizeaza: blocul de statistici din hero (index.html), banda de
cifre cheie, textul de introducere, intrebarile frecvente si pagina
`autostrazi-romania-2026-bilant`.
