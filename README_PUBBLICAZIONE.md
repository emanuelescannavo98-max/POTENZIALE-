# POTENZIALE 1.2 — pubblicazione da smartphone

Questo pacchetto è pronto per essere pubblicato come sito statico HTTPS e poi installato come PWA su Android.

## Metodo consigliato: GitHub Pages

1. Crea/accedi a un account GitHub.
2. Crea un nuovo repository, ad esempio `potenziale`.
3. Carica **tutti i file di questa cartella**, mantenendo anche `.github/workflows/pages.yml` e `.nojekyll`.
4. Vai in **Settings → Pages**.
5. In **Build and deployment → Source** seleziona **GitHub Actions**.
6. Attendi il completamento del workflow `Deploy POTENZIALE to GitHub Pages`.
7. Apri l'URL Pages indicato da GitHub dal tuo Android.
8. In Chrome usa il menu del browser e scegli **Installa app** / **Aggiungi alla schermata Home** (la dicitura può variare).

GitHub Pages pubblica il sito su HTTPS, requisito fondamentale per l'installazione PWA e per il service worker. Il workflow incluso automatizza la pubblicazione a ogni aggiornamento del ramo `main`.

## Dati personali
POTENZIALE salva i dati applicativi nel `localStorage` del dispositivo e offre backup/ripristino JSON. Non inserire password, dati bancari o altre informazioni sensibili nel codice del repository.

## Struttura
- `index.html` — applicazione
- `manifest.json` — configurazione PWA
- `sw.js` — cache/offline
- `icon-192.png`, `icon-512.png` — icone
- `.github/workflows/pages.yml` — deploy GitHub Pages
- `.nojekyll` — pubblicazione statica
