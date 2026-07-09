# TODO - Navigation rapide ↑/↓ sur bras-city-label

## Étape 1 — Préparation
- [x] Comprendre la génération dynamique des `.bras-city-label` dans `script.js`.
- [x] Identifier le conteneur de scroll (`.addresses-cards-container` si présent, sinon `window`).

## Étape 2 — Injection UI
- [ ] Modifier `script.js` pour ajouter 2 boutons à chaque `.bras-city-label` : `↑` et `↓`.
- [ ] Assurer que les boutons ne déclenchent pas l’ouverture/fermeture du `details` (stopPropagation + type=button).

## Étape 3 — Logique navigation
- [ ] Au clic, trouver le label courant et calculer le précédent/suivant parmi les labels pertinents (exclure ceux en `display:none`).
- [ ] Faire scroller vers la cible dans le bon conteneur.
- [ ] Ajouter un léger décalage pour compenser le header fixe.

## Étape 4 — Styling
- [ ] Ajouter styles dans `style.css` (positionnement gauche, taille, hover/focus).
- [ ] Responsive (mobile: boutons compacts, desktop: lisibles).

## Étape 5 — Validation
- [ ] Tester sur mobile et desktop.
- [ ] Tester avec recherche filtrée (labels cachés).
- [ ] Vérifier accessibilité (focus visibles, pas de blocage clic).

