# Run to You
Gioco di avventura per raggiungere un proprio caro. Un gioco Playtale.

El Falcon corre attraverso quattro tappe (Santorini, Ios, Berlino, Vienna) per raggiungere Il Crocco, raccogliendo i ricordi dell'Album. Dopo il viaggio ci sono la sfida dei salamini d'oro e la Partita libera.

## Come si apre
Il gioco è tutto in un file: `index.html`. Basta aprirlo nel browser; si gioca col telefono in orizzontale.
Indirizzo su GitHub Pages: https://marcocipriani08.github.io/Run-to-You/

## Icona e anteprima
- `apple-touch-icon.png` (180 px, iPhone), `icon-192.png` e `icon-512.png` (Android), `icon-maskable-512.png` (Android, con più margine per le maschere tonde), `favicon-32.png` (scheda del browser). Disegno: El Falcon in aria sopra la valigia e il Crocco che arriva per saltarla, sfondo menta.
- `manifest.webmanifest`: aggiunto alla schermata Home, su Android il gioco parte a schermo intero e in orizzontale (iPhone ignora l'orientamento).
- `sw.js`: fa aprire il gioco anche senza connessione dall'icona della Home (solo sulla copia di GitHub Pages). La pagina si scarica dalla rete quando c'è, così gli aggiornamenti arrivano subito; senza rete si usa la copia salvata. I font sono dentro la pagina, non più su Google Fonts.
- `anteprima.png` (1200×630): l'immagine che WhatsApp mostra col link, con titolo «Run to You» e testo «Un piccolo gioco fatto per te.». I tag `og:` usano l'indirizzo assoluto qui sopra: se cambia l'indirizzo, vanno aggiornati.

## Agganci per i test
- `?auto=1` avvia l'autopilota.
- `window.HR` espone `{ G, P, save, LEVELS, go, levelIntro, showBoard, startLevel, setAuto, Bot, pose }`.
