# Pubblicazione del network

## 1. Google Drive e Google Sheets

1. Caricare `parlamento_sardo_network.xlsx` su Google Drive.
2. Aprirlo con Google Fogli e salvarlo come foglio Google nativo.
3. Verificare che i fogli si chiamino esattamente `nodi` e `Connessioni`.
4. Usare **File → Condividi → Pubblica sul web → Intero documento → Pubblica**.
5. Copiare l’ID dall’URL: `https://docs.google.com/spreadsheets/d/ID_DEL_FOGLIO/edit`.

## 2. Configurare l’HTML

Nel file `parlamento_sardo_network.html`, sostituire:

```js
const DEFAULT_SHEET_ID = 'INSERISCI_ID_GOOGLE_SHEET';
```

con l’ID copiato. In alternativa, senza modificare il file, aggiungere `?sheet=ID_DEL_FOGLIO` all’URL della pagina.

## 3. GitHub Pages

1. Caricare `parlamento_sardo_network.html` in un repository GitHub.
2. In **Settings → Pages**, pubblicare dal branch desiderato.
3. Attendere l’URL pubblico, ad esempio `https://utente.github.io/repository/parlamento_sardo_network.html`.

## 4. Incorporare in Drupal

Inserire in un blocco o campo HTML:

```html
<iframe
  src="https://utente.github.io/repository/parlamento_sardo_network.html"
  title="Parlamento sardo: rete di procure e procuratori"
  width="100%"
  height="820"
  style="border:0;display:block"
  loading="lazy"
  allowfullscreen>
</iframe>
```

Se Drupal elimina l’elemento `iframe`, autorizzarlo nella configurazione del formato di testo oppure usare un blocco con HTML completo amministrato.
