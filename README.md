# Copertine Matematica in Rete

Tool web per creare le copertine A4 delle collane LAB Matematica, LAB Fisica e Corso.

Ogni collana mantiene gabbia e colori. Si possono modificare testi e immagini e scaricare il risultato in PNG, JPG, PDF o in un JPG leggero per il sito.

## Come si usa

Il tool è una pagina statica, senza installazione né build. Per provarlo in locale:

```bash
python3 -m http.server 8000
```

Poi apri `http://localhost:8000`. Le copertine restano solo nel browser di chi le crea.

Serve la connessione a internet: pdf-lib e fontkit, usati per il PDF, si caricano da CDN.

## File

- `index.html`: la pagina con interfaccia e logica.
- `font-copertine.js`: il font Inter incluso, con le forme e la spaziatura scelte per le copertine.
- `immagini-esempio.js`: le immagini delle copertine di esempio, a bassa risoluzione. Per la stampa vanno ricaricati gli originali.

## Licenze

Inter è distribuito con licenza SIL Open Font License 1.1. Il testo completo è in testa a `font-copertine.js`.
