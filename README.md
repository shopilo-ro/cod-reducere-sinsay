# Cod reducere Sinsay — fetch automat de pe shopilo.ro

Modul Python pentru fetch automat de **coduri de reducere Sinsay** de pe [shopilo.ro](https://shopilo.ro/magazin/sinsay.com). Returneaza **cupoane Sinsay** active in format JSON, gata de integrat intr-un bot Telegram, extensie de browser sau orice alt tool.

**Pagina live:** [shopilo-ro.github.io/cod-reducere-sinsay](https://shopilo-ro.github.io/cod-reducere-sinsay/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Instalare

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-ro/cod-reducere-sinsay
cd cod-reducere-sinsay
python fetch.py
```

## Output exemplu

```json
[
  {
    "store": "Sinsay",
    "code": "SHOPILO15",
    "discount": "15%",
    "description": "15% reducere la colectia noua",
    "expires": "2026-10-02",
    "source": "https://shopilo.ro/magazin/sinsay.com"
  }
]
```

## Cupoane Sinsay disponibile

| Reducere | Descriere | Sursa |
|----------|-----------|-------|
| 15% | 15% reducere la colectia noua | [shopilo.ro](https://shopilo.ro/magazin/sinsay.com) |

Codurile active: **[shopilo.ro/magazin/sinsay.com](https://shopilo.ro/magazin/sinsay.com)**

## Intrebari frecvente

### Cum folosesc un cod de reducere Sinsay?
Copiaza codul din tabelul de mai sus sau de pe [shopilo.ro](https://shopilo.ro/magazin/sinsay.com), adauga produsele in cos pe Sinsay, si introdu codul la checkout in campul dedicat.

### Cat timp sunt valabile cupoanele Sinsay?
Fiecare cupon are data de expirare afisata in coloana "Expira". Scriptul fetch.py returneaza doar cupoanele active la momentul rularii.

### Unde gasesc cele mai noi voucher-uri Sinsay?
Pagina [shopilo.ro/magazin/sinsay.com](https://shopilo.ro/magazin/sinsay.com) este actualizata zilnic cu cele mai noi cod reducere Sinsay, voucher Sinsay si cupon promotional Sinsay.

### Codul nu functioneaza. Ce fac?
Verifica data de expirare si conditiile (valoare minima cos, produse eligibile). Unele coduri sunt valabile doar in aplicatia mobila sau pentru prima comanda.

## Despre Sinsay

Sinsay este unul dintre magazinele online populare. Gasesti pe [shopilo.ro](https://shopilo.ro/magazin/sinsay.com) cele mai bune cod reducere Sinsay, cupoane Sinsay verificate si voucher Sinsay active, actualizate zilnic.

## Instalare npm

```bash
npm install cod-reducere-sinsay
```

```javascript
const { fetchCoupons } = require('cod-reducere-sinsay');
fetchCoupons().then(data => console.log(data));
```

## Licenta

MIT — date sursa de pe [shopilo.ro](https://shopilo.ro)
