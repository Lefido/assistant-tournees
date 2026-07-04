# TODO - Paramètres "préfixes numéros spéciaux"

## Objectif
Centraliser la logique qui marque les numéros comme "spéciaux" (rouge) en lisant la liste depuis les paramètres utilisateur (localStorage), au lieu d’avoir des `startsWith()` codés en dur.

## Étapes
- [ ] Mettre à jour `index.html` : ajouter un champ dans **Paramètres** pour éditer la liste (CS, PICKUP, PPDC, REEX, T3032, CI) et la sauvegarder dans `localStorage`.
- [ ] Mettre à jour `script.js` : créer `getNumeroPrefixesSpeciaux()` + `estNumeroSpecial(numero)`.
- [ ] Remplacer partout les `numero.startsWith(...)` par l’appel `estNumeroSpecial(numero)` (recherche vocale, OCR, live, PDF, DOCX).
- [ ] Test manuel : vérifier rouge/surlignage + impression après changement de la liste.

