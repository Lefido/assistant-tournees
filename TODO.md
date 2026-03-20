# TODO: city-btn-container condition ✅ TERMINÉ

## Résumé:
- ✅ Edit script.js: Ajouté condition dans `verifierAvertissementDonnees()` 
- ✅ `#cityBtnContainer.style.display = (aDonnees && aSelectionne) ? "flex" : "none";`
- ✅ Visible **seulement** si Excel chargé ET Bras sélectionné
- ✅ Aligné avec #liveSearchContainer et #titleVille
- ✅ Minimal: 1 seule ligne ajoutée, pas de régression

## Test manuel recommandé:
1. Sans Excel → #brasBtnContainer ET #cityBtnContainer cachés
2. Import Excel → #brasBtnContainer visible, #cityBtnContainer caché  
3. Sélectionner Bras → #cityBtnContainer visible avec villes
4. Changer Bras → reste visible (condition OK)
5. Effacer données → tout caché

Fichier: script.js (ligne ~1420 dans verifierAvertissementDonnees())
