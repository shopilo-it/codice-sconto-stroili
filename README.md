# Codice sconto Stroili, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto Stroili** da [shopilo.it](https://shopilo.it/negozi/stroilioro.com). Restituisce **coupon Stroili** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-stroili](https://shopilo-it.github.io/codice-sconto-stroili/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-stroili
cd codice-sconto-stroili
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "Stroili",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% di sconto su gioielli in oro e argento",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/stroilioro.com"
  }
]
```

## Coupon Stroili disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 10% | 10% di sconto su gioielli in oro e argento | [shopilo.it](https://shopilo.it/negozi/stroilioro.com) |

Codici attivi: **[shopilo.it/negozi/stroilioro.com](https://shopilo.it/negozi/stroilioro.com)**

## Domande frequenti

### Come utilizzo un codice sconto Stroili?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/stroilioro.com), aggiungi i prodotti al carrello su Stroili e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon Stroili?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher Stroili piu recenti?
La pagina [shopilo.it/negozi/stroilioro.com](https://shopilo.it/negozi/stroilioro.com) viene aggiornata quotidianamente con i codici sconto Stroili, voucher Stroili e coupon promozionali Stroili piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su Stroili

Stroili e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/stroilioro.com) trovi i migliori codici sconto Stroili, coupon Stroili verificati e voucher Stroili attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-stroili
```

```javascript
const { fetchCoupons } = require('codice-sconto-stroili');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
