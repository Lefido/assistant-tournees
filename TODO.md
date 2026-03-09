# TODO - Transitions Fluides

## ✅ Transitions implémentées :

1. **Bascule Accueil ↔ Paramètres** (script.js + style.css)
   - Transition en fade de 300ms
   - Effet de slide horizontal

2. **Popup vocal** (voice-popup-overlay)
   - Fade in/out avec scale
   - 300ms

3. **Popup résultats** (.popup-overlay)
   - Fade + scale (0.9 → 1)
   - 300ms

4. **Popup caméra, adresse, PDF** (partagent .popup-overlay)
   - Même transition que les résultats

5. **Color picker** (.color-picker-overlay)
   - Fade + scale
   - 300ms

## Notes :
- Les transitions fonctionnent en ajoutant/enlevant la classe `.hidden`
- Le CSS utilise `pointer-events: none/auto` pour éviter les clics pendant les transitions
- Le `.popup-window` et `.color-picker-window` ont un effet de scale pour un effet plus dynamique

