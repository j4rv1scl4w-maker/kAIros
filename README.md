# Light — Blog di Nicolò Marana

Blog personale su **tech, AI e sviluppo software**. Sito statico generato con
[Jekyll](https://jekyllrb.com/) e pubblicato gratuitamente con **GitHub Pages**.

🔗 **Sito:** https://j4rv1scl4w-maker.github.io/light

---

## Come pubblicare un articolo

Ogni articolo è un singolo file Markdown dentro la cartella `_posts/`.

### 1. Nome del file

Deve seguire **esattamente** questo formato:

```
_posts/ANNO-MESE-GIORNO-titolo-con-trattini.md
```

Esempio: `_posts/2026-07-15-il-futuro-degli-agenti-ai.md`

### 2. Contenuto del file

In cima va l'intestazione (il "front matter") tra `---`, poi il testo:

```markdown
---
title: "Titolo dell'articolo"
date: 2026-07-15
tags: [ai, agenti, sviluppo]
description: "Riassunto di 1-2 frasi che appare su Google e quando condividi il link sui social."
---

Qui scrivi il corpo dell'articolo in **Markdown**.

## Un sottotitolo

Testo normale, elenchi, link, immagini, codice... tutto supportato.
```

| Campo         | Obbligatorio | Note                                              |
|---------------|--------------|---------------------------------------------------|
| `title`       | ✅           | Titolo dell'articolo                              |
| `date`        | ✅           | Formato `AAAA-MM-GG` (deve combaciare col file)   |
| `tags`        | ❌           | Elenco di parole chiave tra parentesi quadre      |
| `description` | ❌ (consigliato) | Riassunto per SEO e anteprime social         |

### 3. Pubblicare

Salva il file, fai commit e push. GitHub Pages ricostruisce il sito da solo in
1-2 minuti. **Non serve nessun comando di build.**

> 💡 In alternativa puoi semplicemente passare a Nicolò (o all'assistente) il
> titolo e il testo: il file viene creato e pubblicato per te.

---

## Promemoria Markdown veloce

```markdown
## Titolo grande        ### Titolo medio
**grassetto**           *corsivo*
[testo del link](https://esempio.com)
![descrizione](percorso/immagine.jpg)
- punto elenco          1. elenco numerato
> citazione             `codice inline`
```

---

## SEO e indicizzazione (già configurato)

- ✅ **Sitemap** automatica (`/sitemap.xml`)
- ✅ **Meta tag** Open Graph + Twitter Card su ogni pagina
- ✅ **Feed RSS** (`/feed.xml`)
- ✅ **robots.txt** che invita i motori a indicizzare tutto

Per accelerare l'indicizzazione su Google: registrare il sito su
[Google Search Console](https://search.google.com/search-console) e inviare
l'URL della sitemap.

---

## Sviluppo in locale (opzionale)

```bash
bundle install
bundle exec jekyll serve
# apri http://localhost:4000/light
```

---

## Struttura del progetto

```
_config.yml          Configurazione del sito
_posts/              👈 Gli articoli (un file Markdown ciascuno)
_layouts/            Template HTML delle pagine
_includes/           Header, footer, head riutilizzabili
assets/css/          Stile (dark/tech, mobile-first)
index.html           Home page con la lista degli articoli
about.md             Pagina "Chi sono"
```
