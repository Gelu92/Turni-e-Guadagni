# Turni e Mance

App per segnare turni, paga, mance, entrate, spese e giorni di riposo. Funziona anche senza internet e i dati restano solo sul telefono.

*Gelu Inc.*

## Cosa c'è nella cartella

Tutti i file stanno nella stessa cartella, senza sottocartelle, così si caricano senza problemi anche dal telefono.

| File | A cosa serve |
|---|---|
| `index.html` | L'app |
| `manifest.webmanifest` | Nome, icona e colori per l'installazione |
| `sw.js` | Fa funzionare l'app anche senza internet |
| `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `apple-touch-icon.png` | Le icone |
| `versione-precedente.html` | La versione di prima, da aprire solo se ti serve |

## Pubblicarla su GitHub

1. Nel repository carica **tutti i file** dello zip nella radice, cioè in primo piano, non dentro un'altra cartella. Se c'erano file vecchi (per esempio una cartella `icons`), puoi lasciarli o eliminarli.
2. **Settings → Pages**: *Deploy from a branch*, branch **main**, cartella **/ (root)**. Salva.
3. Aspetta uno o due minuti. Per controllare che le icone ci siano, apri nel browser l'indirizzo del sito seguito da `/icon-192.png`: deve comparire l'icona.

## Installarla sul telefono (Android)

1. Apri l'indirizzo **direttamente in Chrome**, non dal link dentro WhatsApp o Telegram. Se lo apri da lì, tocca ⋮ → **Apri in Chrome**.
2. Se avevi già provato a installarla, prima **disinstalla la vecchia icona**: tienila premuta → *Disinstalla*.
3. Aspetta che la pagina si carichi del tutto e tocca **Installa**: compare la finestra di Chrome, conferma e l'app va sulla schermata Home.

**iPhone (Safari):** pulsante **Condividi** → **Aggiungi alla schermata Home**.

## Aggiornare l'app

Quando carichi una nuova versione di `index.html`, apri `sw.js` e cambia il numero in `turni-e-mance-v2` (v3, v4…). Così il telefono scarica la versione nuova. I tuoi dati non vengono toccati.

## I tuoi dati

Turni, entrate e spese sono salvati solo nel telefono. Fai ogni tanto un **backup** da *Impostazioni → Backup* e tieni il file in un posto sicuro (Drive, email). Se cambi telefono, installa l'app e usa **Importa backup**. Se disinstalli l'app o cancelli i dati di Chrome per quel sito, i dati spariscono: per questo serve il backup.
