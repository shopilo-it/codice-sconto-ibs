# Codice sconto IBS, recupero automatico da shopilo.it

Modulo Python per il recupero automatico di **codici sconto IBS** da [shopilo.it](https://shopilo.it/negozi/ibs.it). Restituisce **coupon IBS** attivi in formato JSON, pronto per l'integrazione in un bot Telegram, estensione del browser o qualsiasi altro strumento.

**Pagina live:** [shopilo-it.github.io/codice-sconto-ibs](https://shopilo-it.github.io/codice-sconto-ibs/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installazione

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-it/codice-sconto-ibs
cd codice-sconto-ibs
python fetch.py
```

## Output di esempio

```json
[
  {
    "store": "IBS",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% di sconto su libri e eBook",
    "expires": "2026-10-10",
    "source": "https://shopilo.it/negozi/ibs.it"
  }
]
```

## Coupon IBS disponibili

| Sconto | Descrizione | Fonte |
|----------|-----------|-------|
| 15% | 15% di sconto su libri e eBook | [shopilo.it](https://shopilo.it/negozi/ibs.it) |

Codici attivi: **[shopilo.it/negozi/ibs.it](https://shopilo.it/negozi/ibs.it)**

## Domande frequenti

### Come utilizzo un codice sconto IBS?
Copia il codice dalla tabella qui sopra o da [shopilo.it](https://shopilo.it/negozi/ibs.it), aggiungi i prodotti al carrello su IBS e inserisci il codice al checkout nel campo dedicato.

### Quanto durano i coupon IBS?
Ogni coupon ha una data di scadenza indicata nella colonna "Scadenza". Lo script fetch.py restituisce solo i coupon attivi al momento dell'esecuzione.

### Dove trovo i voucher IBS piu recenti?
La pagina [shopilo.it/negozi/ibs.it](https://shopilo.it/negozi/ibs.it) viene aggiornata quotidianamente con i codici sconto IBS, voucher IBS e coupon promozionali IBS piu recenti.

### Il codice non funziona. Cosa faccio?
Verifica la data di scadenza e le condizioni (importo minimo del carrello, prodotti idonei). Alcuni codici sono validi solo nell'app mobile o per il primo ordine.

## Informazioni su IBS

IBS e uno dei negozi online piu popolari. Su [shopilo.it](https://shopilo.it/negozi/ibs.it) trovi i migliori codici sconto IBS, coupon IBS verificati e voucher IBS attivi, aggiornati ogni giorno.

## Installazione npm

```bash
npm install codice-sconto-ibs
```

```javascript
const { fetchCoupons } = require('codice-sconto-ibs');
fetchCoupons().then(data => console.log(data));
```

## Licenza

MIT, dati prelevati da [shopilo.it](https://shopilo.it)
