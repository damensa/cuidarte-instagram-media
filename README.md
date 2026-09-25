# cuidarte-instagram-media

Repositori públic d'imatges per als posts d'Instagram. Les URLs públiques dels fitxers es guardaran a Airtable i les consumirà Claude Code dins del flux de publicació.

## Estructura i noms

Una carpeta per setmana ISO, amb el format `AAAA-WNN`, començant per `2026-W40/`.

Fitxers en minúscules, sense espais ni accents:

- Post simple: `ccsc_2026w40_01_reflexion.png`
- Carrusel: `ccsc_2026w40_02_slide1.png`, `ccsc_2026w40_02_slide2.png`, etc.
- Exercici: `ccsc_2026w40_03_ejercicio.png`

El número de dues xifres identifica el post de la setmana; `slide1`, `slide2`, etc. indiquen l'ordre del carrusel.

## URLs públiques

Format amb la branca `main`:

```text
https://raw.githubusercontent.com/damensa/cuidarte-instagram-media/main/2026-W40/ccsc_2026w40_01_reflexion.png
```

A Airtable, el camp proposat `MEDIA_URLS` contindrà una URL per línia, en ordre de diapositives per als carrusels. Claude Code llegirà aquestes URLs per obtenir les imatges.

La URL d'exemple funcionarà quan s'hi pugi el fitxer corresponent. Inicialment no s'inclou cap imatge; `.gitkeep` conserva la carpeta buida.
