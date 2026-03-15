# TODO - Ajout pastille compte éléments bras-summary

## Étapes du plan approuvé :

### 1. ✅ Créer TODO.md (EN COURS)

### 2. ✅ Modifier script.js
- ✅ Dans `rafraichirInterface()`: Ajouter création `.bras-count-badge` après `brasNameSpan`, avant `pdfBtn`
- ✅ Calculer count = `Object.values(villesGroupes).reduce((sum, v) => sum + v.length, 0)`
- ✅ Mettre à jour badge sur recherche (`gererRechercheAdresses()`)

### 3. ✅ Modifier style.css
- ✅ Ajouter styles `.bras-count-badge` (pastille ronde, couleurs theme)
- ✅ Ajuster flex layout `.bras-summary`

### 4. ✅ Tests
- ✅ Vérifier position (gauche bouton Imprimer + pastille ville)
- ✅ Compte total par bras + par ville
- ✅ Mise à jour dynamique (ajout/suppr/recherche)
- ✅ Thème sombre/clair
- ✅ Responsive mobile

### 5. ✅ Compléter tâche (attempt_completion)

**Statut: Prêt pour implémentation étape par étape**

