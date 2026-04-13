# Code promo ManoMano, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo ManoMano** depuis [shopilo.fr](https://shopilo.fr/reductions/manomano.fr). Renvoie les **coupons ManoMano** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-manomano](https://shopilo-fr.github.io/code-promo-manomano/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-manomano
cd code-promo-manomano
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "ManoMano",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% de reduction sur le bricolage et le jardinage",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/manomano.fr"
  }
]
```

## Coupons ManoMano disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 10% | 10% de reduction sur le bricolage et le jardinage | [shopilo.fr](https://shopilo.fr/reductions/manomano.fr) |

Codes actifs : **[shopilo.fr/reductions/manomano.fr](https://shopilo.fr/reductions/manomano.fr)**

## Questions frequentes

### Comment utiliser un code promo ManoMano ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/manomano.fr), ajoutez les produits a votre panier sur ManoMano et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons ManoMano ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction ManoMano les plus recents ?
La page [shopilo.fr/reductions/manomano.fr](https://shopilo.fr/reductions/manomano.fr) est mise a jour quotidiennement avec les codes promo ManoMano, bons de reduction ManoMano et coupons promotionnels ManoMano les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de ManoMano

ManoMano est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/manomano.fr), retrouvez les meilleurs codes promo ManoMano, coupons ManoMano verifies et bons de reduction ManoMano actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-manomano
```

```javascript
const { fetchCoupons } = require('code-promo-manomano');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
