# Sebastian Wyderka

Strona wizytówka. Hurt warzyw i owoców ekologicznych oraz warzyw konwencjonalnych,
konsulting i bezpieczeństwo żywności. Cztery języki: polski, angielski, niemiecki, ukraiński.

```
index.html     cała strona: HTML, CSS, teksty
img/           zdjęcia
```

Strona statyczna, bez backendu i bez budowania. `index.html` leży w korzeniu
repozytorium, więc w Vercelu **Root Directory zostaje puste**, Framework Preset
**Other**, Build Command i Output Directory puste.

## Zmiana tekstów

Teksty siedzą w jednym miejscu, na dole `index.html`, w bloku `const I18N = {...}`.
Każdy język ma ten sam zestaw kluczy. Zmieniasz tekst, commitujesz, Vercel publikuje sam.

## Własna domena

Vercel → projekt → Settings → Domains → Add.

Po podpięciu domeny warto podmienić w `<head>` linijkę
`<meta property="og:image" content="img/hero.jpg">` na pełny adres,
np. `https://twojadomena.pl/img/hero.jpg`, żeby przy wysyłaniu linku
w komunikatorach pokazywała się miniatura.

## Zdjęcia

Z Unsplash, na darmowej licencji, także do użytku komercyjnego.
