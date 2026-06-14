# Cozlo

Convertisseur de relevés bancaires PDF en CSV, entièrement dans le navigateur.

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
| BNP Paribas | 🔄 Parser intégré (non testé sur relevé réel) |
| Société Générale | 🔄 Parser intégré (non testé sur relevé réel) |
| Caisse d'Épargne | 🔄 Parser intégré (non testé sur relevé réel) |
| La Banque Postale | 🔄 Parser intégré (non testé sur relevé réel) |
| Crédit Mutuel | 🔄 Parser intégré (non testé sur relevé réel) |
| LCL | 🔄 Parser intégré (non testé sur relevé réel) |
| Autres | 🔄 Parser générique (résultats variables) |

D'autres banques seront ajoutées. Si votre format n'est pas reconnu, [contactez-nous](mailto:hmanuel515@hotmail.fr) avec un exemple anonymisé.

---

## Tarif

**15 € — accès à vie, paiement unique.**

La conversion est gratuite et illimitée. Le téléchargement CSV nécessite une licence.

[→ Acheter sur Gumroad](https://manuel515.gumroad.com/l/cozlo)

---

## Vie privée & conformité

Cozlo n'envoie aucune donnée à un serveur. Tout le traitement se passe dans votre navigateur via [PDF.js](https://mozilla.github.io/pdf.js/) (Mozilla). Le fichier PDF ne quitte jamais votre appareil. Conforme RGPD par design.

---

## Stack

- HTML / CSS / JS vanilla — aucun framework, aucun build tool
- [PDF.js 3.11](https://mozilla.github.io/pdf.js/) via CDN pour l'extraction du texte
- [Gumroad](https://gumroad.com) pour la gestion des licences

---

## Contact

Un bug ? Une banque non supportée ? → [hmanuel515@hotmail.fr](mailto:hmanuel515@hotmail.fr)
