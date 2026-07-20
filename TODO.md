# Plan d'implémentation : Navigation entre les bras-city-label dans Paramètres

## Problème
- `.bras-city-label` dans `<details>` avec `position: sticky` et `height:16px` → comportement cross-browser instable
- Pas de navigation rapide entre les villes
- Mauvaise expérience sur mobile

## Étapes

### 1. Style CSS ✅
- [x] Supprimer `height: 16px; position: sticky; top: 99px; z-index: 8` de `.bras-city-label`
- [x] Ajouter `scroll-margin-top: 132px` sur `.bras-city-label` pour ancrage fluide
- [x] Ajouter styles du conteneur `.bras-city-btns` (barre de navigation rapide sticky top:99px)
- [x] `flex-wrap: nowrap` + `overflow-x: auto` pour scroll horizontal (gain de hauteur)
- [x] `padding` réduit (4px au lieu de 6px) pour compacter
- [x] Styles des boutons `.city-quick-jump-btn`
- [x] Style bouton actif `.city-quick-jump-btn.active`
- [x] Compatibilité thème sombre (night-theme)

### 2. JavaScript ✅
- [x] Injecter `.bras-city-btns` dans chaque `.bras-details` après le `.bras-summary`
- [x] Créer un bouton par ville avec scrollIntoView au clic
- [x] Marquer le bouton actif avec classe `.active`
- [x] Ajouter écouteur de scroll (Intersection Observer) pour highlight auto
- [x] Synchro avec recherche adresse : filtrer les boutons visibles dans `gererRechercheAdresses()`
- [x] Restaurer boutons quand la recherche est effacée

### 3. Tests ✅
- [x] Vérifier navigation desktop
- [x] Vérifier navigation mobile
- [x] Vérifier compatibilité thème sombre
- [x] Vérifier qu'après ajout/modification/suppression d'adresse, la nav est bien reconstruite
- [x] Vérifier que le filtrage addressSearchInput masque/affiche les boutons correspondants
