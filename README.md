# Cozlo

Convertisseur de relevés bancaires PDF vers CSV, entièrement dans le navigateur.

Aucune donnée ne quitte votre appareil — le traitement est 100% local, sans serveur, sans compte.

**[→ Ouvrir l'outil](https://mano515.github.io/cozlo/)**

---

## Ce que ça fait

1. Glissez un relevé bancaire PDF dans la page
2. Cozlo extrait les transactions, détecte les colonnes Débit / Crédit et nettoie les libellés
3. Vous obtenez un tableau prévisualisable et modifiable
4. Téléchargez le CSV en un clic — prêt pour Excel, Google Sheets ou votre outil de compta

---

## Fonctionnalités

- **Extraction positionnelle** — utilise les coordonnées X/Y du PDF pour distinguer débit et crédit, pas seulement le texte brut
- **Libellés nettoyés** — supprime les préfixes bancaires (`Carte X7621`, `Prlv`, `Vir Inst de`) et les dates redondantes
- **Catégorisation automatique** — Achat CB, Prélèvement, Virement, Retrait, Remboursement
- **Résumé financier** — solde d'ouverture / clôture, total débits, total crédits
- **Colonnes triables** — clic sur un en-tête pour trier
- **Cellules éditables** — corrigez une valeur directement dans le tableau avant d'exporter
- **Multi-relevés** — ajoutez plusieurs PDF successivement pour générer un CSV annuel complet
- **Détection PDF scanné** — message d'erreur clair si le PDF ne contient pas de texte extractible

---

## Banques supportées

| Banque | Statut |
|---|---|
| Crédit Agricole | ✅ Testé |
| Autres | 🔄 Parser générique (résultats variables) |

D'autres banques seront ajoutées. Si votre format n'est pas reconnu, ouvrez une issue avec un exemple anonymisé.

---

## Utilisation

Pas d'installation. Ouvrez simplement `index.html` dans un navigateur, ou utilisez la version hébergée :

```
https://mano515.github.io/cozlo/
```

Pour lancer localement :

```bash
git clone https://github.com/Mano515/cozlo.git
cd cozlo
# Ouvrir index.html dans votre navigateur
```

---

## Vie privée

Cozlo n'envoie aucune donnée à un serveur. Tout le traitement se passe dans votre navigateur via [PDF.js](https://mozilla.github.io/pdf.js/) (Mozilla). Le fichier PDF ne quitte jamais votre appareil.

---

## Stack

- HTML / CSS / JS vanilla — aucun framework, aucun build tool
- [PDF.js 3.11](https://mozilla.github.io/pdf.js/) via CDN pour l'extraction du texte

---

## Licence

MIT
