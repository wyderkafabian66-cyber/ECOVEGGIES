# Strona Sebastian Wyderka

Statyczna strona wizytówka. Brak backendu, brak zależności, nic się nie kompiluje.
Wystarczy wrzucić te pliki na serwer.

```
index.html     cała strona (HTML, CSS, teksty PL/EN/DE/UA)
img/           zdjęcia
```

## Wrzucenie na GitHub

1. Wejdź na https://github.com/new i utwórz repozytorium, np. `sebastian-wyderka`.
   Zostaw je puste, bez README.
2. Na stronie nowego repozytorium kliknij **uploading an existing file**.
3. Przeciągnij plik `index.html` oraz katalog `img` z tego folderu.
4. Kliknij **Commit changes**.

Jeśli wolisz terminal:

```bash
git init
git add .
git commit -m "Strona Sebastian Wyderka"
git branch -M main
git remote add origin https://github.com/UZYTKOWNIK/sebastian-wyderka.git
git push -u origin main
```

## Publikacja na Vercel

1. Wejdź na https://vercel.com i zaloguj się przez GitHub.
2. **Add New** → **Project** → wybierz repozytorium `sebastian-wyderka` → **Import**.
3. Framework Preset zostaw na **Other**, Build Command i Output Directory zostaw puste.
4. **Deploy**. Po chwili dostaniesz adres `nazwa.vercel.app`.

Każdy kolejny commit na GitHubie publikuje się automatycznie.

## Własna domena

Vercel → projekt → **Settings** → **Domains** → **Add**. Wpisz domenę i ustaw
u rejestratora rekordy, które pokaże Vercel.

## Zmiana tekstów

Teksty są w jednym miejscu w `index.html`, w bloku `const I18N = {...}` na dole pliku.
Każdy język ma ten sam zestaw kluczy. Zmieniasz tekst, commitujesz, Vercel publikuje.

Po podpięciu domeny warto podmienić w `<head>` linijkę
`<meta property="og:image" content="img/hero.jpg">` na pełny adres,
np. `https://twojadomena.pl/img/hero.jpg`, żeby miniatura pokazywała się przy
wysyłaniu linku w komunikatorach.

## Zdjęcia

Zdjęcia pochodzą z Unsplash i są na darmowej licencji, także do użytku komercyjnego.
Podpis autorów jest w stopce strony, licencja go nie wymaga, więc można go usunąć.
