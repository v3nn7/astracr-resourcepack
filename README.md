# astraCR resource pack

Publiczna paczka zasobów z ikonami rang dla pluginu **astraCR** (Minecraft 1.21.11, `pack_format` 75).
Ikony są generowane przez plugin (zaokrąglone plakietki z napisem), a glify leżą w czcionce `minecraft:default`
(znaki z prywatnego zakresu Unicode `U+E000`+), więc działają w czacie, TAB-ie i przez placeholdery.

| Ranga | Znak |
|---|---|
| owner | `U+E000` |
| admin | `U+E001` |
| moderator | `U+E002` |
| helper | `U+E003` |
| mvp | `U+E004` |
| vip | `U+E005` |
| gracz | `U+E006` |
| media | `U+E007` |

## Użycie w astraCR

W `plugins/astraCR/ranks.yml`:

```yaml
pack:
  external-url: "https://raw.githubusercontent.com/v3nn7/astracr-resourcepack/main/astracr-badges.zip"
```

Plugin liczy SHA-1 z lokalnie zbudowanej paczki. Zbudowana z domyślnego `ranks.yml` jest identyczna z plikiem
w tym repo (SHA-1: `e2f064068199883fa43a05eb36ac98d44f2f4dbb`). Jeśli zmienisz rangi, kolory lub napisy, zbuduj paczkę ponownie
(`/astracr pack build`) i wgraj tu `plugins/astraCR/pack/astracr-badges.zip`, inaczej klienci odrzucą paczkę przez
niezgodny hash.

## Zawartość

- `astracr-badges.zip` – gotowa paczka do pobrania
- `astracr-badges.zip.sha1` – suma kontrolna
- `pack-contents/` – ta sama paczka rozpakowana (`pack.mcmeta`, `assets/minecraft/font/default.json`, tekstury w `assets/astracr/textures/badge/`)
