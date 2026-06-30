# Experiences

Een verzameling kleine, op zichzelf staande interactieve mini-apps, gebouwd met pure HTML, CSS en JavaScript — zonder build-stap, framework of backend. De site wordt automatisch gedeployed naar GitHub Pages.

## Experiences

| Experience | Beschrijving |
| --- | --- |
| 🎨 Kleurmixer | Mix RGB-kleuren en kopieer HEX-waarden naar je klembord. |
| 🧠 Geheugenspel | Onthoud de reeks knopflitsen en herhaal zo lang mogelijk. |
| 🕐 Woordklok | De huidige tijd weergegeven in Nederlandse woorden. |
| ✏️ Tekenveld | Teken vrij op een canvas met penseel en kleurenkeuze. |
| ⚡ Reactietest | Test je reactiesnelheid: klik zo snel mogelijk als het veld groen wordt. |

## Structuur

- `index.html` — homepage met een tegelgrid naar alle experiences
- `style.css` — gedeelde stijl (kleurvariabelen, navigatie, tegelgrid, knoppen)
- `experiences/` — de losse mini-apps, elk een zelfstandige HTML-pagina
- `.github/workflows/deploy.yml` — GitHub Actions workflow die de site bij elke push naar `main` naar GitHub Pages deployt

## Lokaal bekijken

Het is een statische site, dus open `index.html` direct in je browser, of serveer de map lokaal:

```bash
python3 -m http.server 8000
```

Ga vervolgens naar `http://localhost:8000`.

## Deployment

Bij elke push naar de `main`-branch deployt de GitHub Actions workflow de inhoud van de repository automatisch naar GitHub Pages.
