# Portfolio — jak wystawić na żywo

Plik `index.html` to gotowa, statyczna strona (HTML + CSS + JS, three.js z CDN, zdjęcia osadzone w środku). Nie wymaga budowania ani backendu — wystarczy go wrzucić na hosting statyczny.

## Nazwa repozytorium / linku

Zaproponowana nazwa repo (i tym samym adresu):

```
bartosz-guderski-portfolio
```

Po wrzuceniu na GitHub Pages Twój adres będzie wyglądał tak:

```
https://twoj-login-github.github.io/bartosz-guderski-portfolio/
```

## Krok po kroku — GitHub Pages

1. Wejdź na github.com/new i utwórz nowe repozytorium o nazwie **`bartosz-guderski-portfolio`** (publiczne).
2. Wrzuć do niego plik `index.html` z tego folderu (przez interfejs GitHuba: **Add file → Upload files**, albo przez `git`, jeśli wolisz terminal).
3. Wejdź w **Settings → Pages** tego repozytorium.
4. W sekcji **Build and deployment → Source** wybierz **Deploy from a branch**, branch: `main`, folder: `/ (root)` → **Save**.
5. Po ok. minucie strona pojawi się pod adresem:
   `https://twoj-login-github.github.io/bartosz-guderski-portfolio/`
6. Jeśli chcesz własną domenę (np. `bartoszguderski.pl`) — w tej samej zakładce **Custom domain** wpisz swoją domenę i dodaj u dostawcy domeny rekord `CNAME` wskazujący na `twoj-login-github.github.io`.

## Alternatywa — Railway

Railway lepiej sprawdza się przy projektach z backendem, ale statyczną stronę też da się tam wystawić:

1. Nowy projekt → **Deploy from GitHub repo** → wskaż `bartosz-guderski-portfolio`.
2. Jeśli Railway poprosi o start command, dodaj plik `package.json`:
   ```json
   {
     "scripts": { "start": "npx serve -s . -l $PORT" }
   }
   ```
3. Po deployu dostaniesz adres `*.up.railway.app`, do którego również można podpiąć własną domenę (**Settings → Domains**).

## Rekomendacja

Do gotowego portfolio **GitHub Pages jest szybsze i wystarczające** — nazwa repo `bartosz-guderski-portfolio` od razu ładnie się prezentuje w linku.
