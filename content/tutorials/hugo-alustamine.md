---
title: "Hugo Alustamine"
date: 2026-01-15
draft: false
---

# Kuidas alustada Hugo'ga

Hugo on kiire ja paindlik staatiline veebilehe generaator, mis on kirjutatud Go keeles.

## Paigaldamine

Hugo saab paigaldada mitmel viisil:

- **macOS**: `brew install hugo`
- **Windows**: Laadi alla `.exe` fail Hugo lehelt
- **Linux**: Kasuta pakihaldur või laadi alla binaarfail

## Uue saidi loomine

Uue Hugo saidi loomiseks kasuta käsku:

```bash
hugo new site minu-sait
cd minu-sait
```

## Teema lisamine

Hugo vajab teemat, et sait korralikult välja näeks:

```bash
git submodule add https://github.com/budparr/gohugo-theme-ananke.git themes/ananke
echo "theme = 'ananke'" >> config.toml
```

## Sisu loomine

Uue postituse loomiseks:

```bash
hugo new posts/minu-esimene-postitus.md
```

## Kohaliku serveri käivitamine

Vaata oma saiti brauseris:

```bash
hugo server -D
```

Ava brauser aadressil `http://localhost:1313`

## Saidi ehitamine

Staatiline sait luuakse käsuga:

```bash
hugo
```

Valmis failid on `public/` kataloogis.
