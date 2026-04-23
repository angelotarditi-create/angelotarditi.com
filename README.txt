ANGELO TARDITI — sito personale
================================

STRUTTURA FILE
├── index.html          → la pagina unica
├── favicon.svg         → favicon vettoriale (monogramma AT)
├── favicon.ico         → fallback favicon (16/32/48 px)
├── apple-touch-icon.png → icona iOS (180×180)
├── og-image.jpg        → anteprima social (1200×630)
└── assets/             → le 13 immagini (una per lettera)
    ├── 01.jpg → A  Da piccolo giocavo a fare il lavoro che faccio oggi
    ├── 02.jpg → N  Ingegneria del cinema / Brand storytelling
    ├── 03.jpg → G  Wearable Tech Torino
    ├── 04.jpg → E  Primo giorno in Eggers ("Sto in fissa")
    ├── 05.jpg → L  Gli amici dell'università
    ├── 06.jpg → O  Visionary Days – prima edizione (11/11/2017)
    ├── 07.jpg → T  Visionary Days – seconda edizione
    ├── 08.jpg → A  Pagina intera su La Stampa
    ├── 09.jpg → R  Piano editoriale fisico (post-it)
    ├── 10.jpg → D  Videochiamata con Mattarella
    ├── 11.jpg → I  #UnoNonBasta – proiezione su Palazzo Chigi
    ├── 12.jpg → T  Campagna per candidato fake (Giovanni Assenti)
    └── 13.jpg → I  Sala regia / il prossimo capitolo

COME METTERLO ONLINE
--------------------
Il sito è 100 % statico: basta caricare l'intera cartella su qualsiasi
hosting (Netlify, Vercel, GitHub Pages, Aruba, un qualsiasi FTP).

- Netlify / Vercel: trascina la cartella sulla dashboard.
- GitHub Pages: push della cartella in un repo, Settings → Pages → branch main.
- Hosting classico: carica tutto via FTP nella root del dominio.

ANTEPRIMA LOCALE
----------------
Da terminale, dentro la cartella:
    python3 -m http.server 8000
poi apri http://localhost:8000

PERSONALIZZAZIONE RAPIDA
------------------------
- Testi dei capitoli: array `captions` nel tag <script> in fondo a index.html
- Colori: variabili CSS nel :root all'inizio dello <style>
    --paper  (sfondo chiaro)
    --ink    (testo principale)
    --accent (puntino arancione, hover default)
- Font: Fraunces (titolo) + Instrument Sans (testo) caricati da Google Fonts
- Sostituzione immagini: mantieni gli stessi nomi (01.jpg → 13.jpg) in /assets

NOTE TECNICHE
-------------
- Desktop: hover sulle lettere
- Mobile/Touch: tap singolo per attivare, tap fuori per chiudere
- Tastiera: Tab per navigare tra le lettere, Invio/Spazio per attivare, Esc per chiudere
- Reduced motion: le transizioni sono ridotte automaticamente per chi lo preferisce
- Tutte le immagini sono in preload per transizioni fluide
