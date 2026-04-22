# Parkour A.p.s. — Sito vetrina

Sito vetrina a pagina singola per Parkour A.p.s., associazione di promozione sociale con sede a Torino.

## Contenuto della cartella

- `index.html` — homepage del sito
- `parkour-preview.png` — immagine di anteprima (1200×630) per Google, Facebook, WhatsApp, LinkedIn, Twitter/X
- `favicon.ico` — icona multi-risoluzione per i browser (16/32/48 px)
- `favicon-16x16.png`, `favicon-32x32.png`, `favicon-48x48.png` — favicon PNG per browser moderni
- `apple-touch-icon.png` — icona 180×180 per la home screen di iPhone/iPad
- `README.md` — questo file

## Come vedere il sito in locale

Basta aprire `index.html` con il browser (doppio click sul file).

## Come pubblicarlo online

1. Carica `index.html` e `parkour-preview.png` nella stessa cartella sul server web (stesso livello).
2. **Importante**: una volta che conosci l'URL definitivo del sito (es. `https://parkour-aps.it/`), apri `index.html` e sostituisci **tutte** le occorrenze di `parkour-preview.png` con l'URL assoluto dell'immagine (es. `https://parkour-aps.it/parkour-preview.png`). Serve perché Facebook, WhatsApp e gli altri social richiedono URL completi per mostrare l'anteprima quando qualcuno condivide il link.

Le righe da modificare sono queste tre nell'`<head>`:

```html
<meta property="og:image" content="parkour-preview.png">
...
<meta name="twitter:image" content="parkour-preview.png">
```

## Avviso assemblea

Il box in hero contiene la convocazione dell'Assemblea Ordinaria dei Soci:
**lunedì 27 aprile 2026, ore 17:00** (prima convocazione) / **ore 18:00** (seconda convocazione).

Dopo la data, ricordati di aggiornare o rimuovere l'avviso (si trova nell'HTML dentro `<div class="notice">`).

## Dati APS

- Parkour A.p.s.
- Via Lancia 138/2 — 10141 Torino
- CF 97910760012

## Note tecniche

- Il video di sfondo è embeddato da YouTube (video ID `z6DY5GbrH5I`). Se l'autore del video disabilita l'autoplay o rimuove il video, sostituisci il video ID nell'iframe dentro `index.html` (due occorrenze nella stessa riga).
- Il sito usa font Google caricati via CDN (Anton, Archivo, JetBrains Mono): richiede connessione internet dell'utente finale.
- Nessuna dipendenza da framework: HTML + CSS puro, funziona ovunque.
