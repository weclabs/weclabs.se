# W.E.C Labs AB – webbplats

Enkel webbplats (vanliga HTML-filer, inget att bygga) som uppfyller Apples krav för Apple Developer Program: riktig information om bolaget, juridiskt namn, org.nr, adress och kontakt, integritetspolicy, villkor och support. Svenska i roten och engelska i `en/`.

Arbetsnamn för domänen: **weclabs.se** (ledig 2026-11-01). Byts domänen, ändra i `CNAME` och byt `kontakt@weclabs.se` i alla .html-filer.

## Publicera (GitHub Pages, gratis, med HTTPS)

Allt som kräver inloggning eller betalning gör Wenche själv.

1. **Domän (Loopia):** registrera `weclabs.se` med **W.E.C Labs AB (559508-2347)** som innehavare, inte privatperson. Lägg till e-post (Loopia Mail eller vidarebefordran) för `kontakt@weclabs.se`.
2. **GitHub:** skapa en organisation för bolaget (Free), `weclabs` (skapad 2026-11-01), på github.com/organizations/plan.
3. **Ladda upp:** Claude skapar repot `weclabs/weclabs.se` (offentligt, eftersom webbplatsen är offentlig) och laddar upp filerna, efter Wenches godkännande.
4. **Slå på Pages:** repot → Settings → Pages → Source: *Deploy from a branch*, `main`, `/ (root)`. Custom domain: `weclabs.se`.
5. **DNS hos Loopia** (Loopia Customer Zone → domänen → DNS-editor). Låt MX-posterna för e-posten vara kvar.
   - `@` A → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `www` CNAME → `weclabs.github.io.`
6. Vänta tills GitHub visar att DNS-kontrollen är klar (minuter till några timmar). Kryssa sedan i **Enforce HTTPS**.
7. Rekommenderat: verifiera domänen i organisationen (Settings → Pages → Add a domain), så att ingen annan kan använda den på GitHub.

## Ändra texter

Öppna .html-filen, ändra texten och ladda upp igen. Varje sida har en svensk och en engelsk version, så ändra båda.
