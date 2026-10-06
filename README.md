# ArredamiTU

Web app personale per seguire lavori, arredamento e budget della casa nuova (Cristian e Paola).

## Pubblicazione su GitHub Pages
1. Crea un nuovo repository su GitHub (es. `arredamitu`), anche privato se hai un piano che lo consente, altrimenti pubblico.
2. Carica **tutti** i file di questa cartella mantenendo la struttura (`index.html`, `manifest.json`, `sw.js`, cartella `icons/`).
3. Vai in **Settings → Pages**, alla voce *Source* scegli **Deploy from a branch**, branch `main`, cartella `/ (root)`, e salva.
4. Dopo un paio di minuti l'app è su `https://<tuo-utente>.github.io/arredamitu/`.
5. Aprila dal telefono e installala: su iPhone Safari → Condividi → *Aggiungi alla schermata Home*; su Android Chrome → ⋮ → *Installa app*.

## Dati
I dati restano solo sul dispositivo (memoria del browser). Da **Impostazioni** puoi esportare e importare un backup JSON: fallo ogni tanto, e sempre prima di cambiare telefono o cancellare i dati del browser.

## Aggiornamenti
Quando carichi una nuova versione di `index.html`, incrementa anche `CACHE` in `sw.js` (es. `arredamitu-v2`) così il telefono scarica subito la versione nuova.

## Casa in 3D
`casa3d.html` è il modello 3D della casa (pareti dalla Tavola 3, elementi fissi e arredo deciso). Si apre dalla scheda **Stanze** con il pulsante *Vedi in 3D*: se è selezionata una stanza, il 3D parte già inquadrato su quella stanza. La libreria 3D (three.js r128) è nella cartella `vendor/`, così funziona anche offline una volta aperta la prima volta.

Quando il modello viene aggiornato, sostituisci `casa3d.html` e incrementa `CACHE` in `sw.js`.
