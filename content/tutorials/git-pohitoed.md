---
title: "Git Põhitõed"
date: 2026-01-15
draft: false
---

# Git põhitõed algajatele

Git on versioonihaldustööriist, mis aitab koodimuudatusi jälgida ja meeskonnatööd teha.

## Põhilised käsud

### Repository kloonimine

```bash
git clone https://github.com/kasutajanimi/repo-nimi.git
```

### Muudatuste lisamine

```bash
# Vaata staatust
git status

# Lisa failid staging'sse
git add failinimi.txt

# Lisa kõik muudetud failid
git add .
```

### Commit'imine

```bash
git commit -m "Kirjeldav teade muudatuste kohta"
```

### Push ja Pull

```bash
# Saada muudatused serverisse
git push origin main

# Hangi viimased muudatused
git pull origin main
```

## Harude kasutamine

```bash
# Loo uus haru
git branch uus-funktsioon

# Lülitu harule
git checkout uus-funktsioon

# Või mõlemad korraga
git checkout -b uus-funktsioon
```

## Abiks

```bash
# Vaata käsu abi
git help <käsk>

# Näiteks
git help commit
```

Git on võimas tööriist - alguses võib tunduda keeruline, aga praktika teeb meistriks!
