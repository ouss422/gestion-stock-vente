# Gestion de vente et de stock

Application web (HTML/CSS/JS, sans serveur) : tableau de bord, produits, ventes (panier), rapports, alertes, commandes, comparaison de prix, fournisseurs, clients, paramètres.

## Mise en ligne sur GitHub Pages
1. Créez un dépôt GitHub et déposez `index.html` et `data.json` (et, si vous le souhaitez, `produits-initiaux.xlsx` et `donnees-initiales.xlsx`) **à la racine**.
2. Dépôt → **Settings → Pages** → *Deploy from a branch* → branche `main`, dossier `/ (root)` → Save.
3. Le site est disponible sur `https://<compte>.github.io/<depot>/`.

## État initial
L'application démarre **vide** : aucun produit, vente, client ni fournisseur ; chiffre d'affaires à 0.
- `produits-initiaux.xlsx` : liste des produits d'origine (page Produits → « Remplir le tableau (Excel) »).
- `donnees-initiales.xlsx` : ventes, fournisseurs et clients d'origine (consultation).

## Utilisation par d'autres boutiques / domaines
- **Nom, icône et devise** : page « Paramètres » (le nom apparaît dans le menu, l'onglet et les impressions).
- Valeurs par défaut au premier lancement : champs `appName`, `appIcon` et `currency` de `data.json`.
- **Catégories** : page Produits → « Gérer les catégories » (ajout, renommage, suppression), ou directement dans chaque ligne du tableau.
- Pour une autre boutique : déposez `index.html` et un `data.json` avec vos propres valeurs. Les fichiers Excel d'origine sont facultatifs (leurs boutons de téléchargement ne fonctionneront que si les fichiers sont présents).

## Données
Les données sont enregistrées dans le navigateur (localStorage). Exportez régulièrement une sauvegarde JSON depuis la page **Données** ; elle permet aussi de changer d'appareil.
