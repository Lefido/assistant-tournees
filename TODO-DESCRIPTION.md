# DESCRIPTION DU SITE - ASSISTANT TOURNÉES (Pour les nulls 🤪)

## 🎯 **QU'EST-CE QUE C'EST ?**
**Assistant Tournées** = Application web **PWA** (Progressive Web App) pour **La Poste** - **gestion ultra-simple des tournées de distribution**.

**Logo** : Sniper (assets/snipers.png) → \"Précision chirurgicale\" pour trouver les adresses ! 🥷

**Thème** : Bleu La Poste + **dark mode** automatique + **PWA installable** (manifest.json)

---

## 🏠 **ACCUEIL (Mode par défaut)**

### 1. **Sélection BRAS** (obligatoire)
```
[Boutons bleus : Bras 1, Bras 2, Bras 3...]
```
→ **Cliquez un BRAS** → Active (bleu) → **Recherche activée !**

### 2. **VILLES** (optionnel - apparaît après BRAS)
```
[Paris, Lyon, Marseille...]
```
→ **Filtre fin** (clic toggle ON/OFF)

### 3. **RECHERCHE** (zone principale)
```
🎤 MICRO + [Champ texte] + 🗑️
```
- **Tapez** \"paix\" → **Résultats groupés PAR VILLE**
- **Micro** → Dites \"RUE DE LA PAIX\" → **Popup confirme \"PAIX ?\"** → OK
- **Type 1** (exact) → **Type 2** (approx si vide)

**Résultats** :
```
📍 PARIS
→ Rue de la Paix     10-25
→ Rue de la Paix     CS    ← ROUGE (spéciaux)
📍 LYON
→ Rue de la Paix     30
```

---

## ⚙️ **PARAMÈTRES** (Bouton engrenage 🔄)

### **Toggles** :
```
☀️ Thème sombre  [ON/OFF]
📷 Caméra OCR    [ON/OFF]  ← Bouton 📸 apparaît
```

### **Données** :
```
📥 IMPORTER Excel  ← .xlsx (BRAS | Ville | Adresse | Numéro | Type)
📤 EXPORTER Excel
📓 JOURNAL (avec compteur)
➕ AJOUTER adresse
🗑️ EFFACER tout
```

**Champs Excel obligatoires** :
```
BRAS | Ville | Adresse | Numéro de tournée | Type Recherche (1/2)
Ex:  \"1\" | \"paris\" | \"rue de la paix\" | \"10 à 25\" | \"1\"
```

### **Gestion adresses** (CRUD complet)
```
BRAS 1 ▼
  🏙️ PARIS (12)
  → [Rue...] 10-25 ✏️🗑️
  → [Rue...] CS   ✏️🗑️ ← ROUGE
  🖨️ [Imprimer]
```
- **Clic carte** → **Modifier** (popup)
- **🗑️** → Supprimer
- **➕** → Ajouter (popup complète)

**Recherche** dans admin : tapez → **Filtre live** + **badges mis à jour**

---

## 🎤 **RECHERCHE VOCALE**
1. **BRAS sélectionné** → **🎤**
2. **Dites** \"RUE DE LA PAIX\"
3. **Popup** : \"Mot détecté **PAIX** ?\"
   - ✅ **Confirmer** → Recherche
   - 🔄 **Réessayer**
   - ❌ **Annuler**

---

## 📷 **CAMÉRA OCR** (toggle ON)
1. **📷** → **Popup caméra**
2. **Zone verte** → Visez **\"10 Rue Paix\"**
3. **Capturer** → **Extrait auto** → **Recherche !**

**HTTPS obligatoire** (micro + caméra)

---

## 🖨️ **IMPRESSION** (bouton 🖨️ dans chaque BRAS)
```
Sélection villes - BRAS 1
⚪ PARIS  [pastille couleur] (12)
⚪ LYON   [pastille couleur] (8)
```
- **Pastille** → **Changer couleur** (16 couleurs)
- **PDF A3/A4** → **Première lettre ROUGE** + **CS/PICKUP en surligné**
- **Word .docx** → Même format

**Sortie** :
```
PARIS (couleur)
R**UE** Paix     10-25
R**UE** Paix     CS     ← ROUGE/SURLIGNÉ
```

---

## 💾 **PERSISTANCE**
- **localStorage** : Adresses + Sélections + Couleurs + Journal
- **Journal** : Création/Modif/Suppr (export Excel)
- **Auto-restore** : Bras + Onglet (Accueil/Paramètres)

---

## 📱 **PWA / RESPONSIVE**
- **Installable** (manifest.json)
- **Tactile OK** (vibrations)
- **Mobile/Desktop**
- **Font Awesome** + **XLSX.js** + **Tesseract OCR**

---

## 🚀 **ASTUCES PRO**
```
• Recherche 2-3 lettres = assez !
• CS/PICKUP/PPDC/REEX/CI = ROUGE auto
• Type 2 = fallback si Type 1 vide
• Sauvegarde auto (fermeture/refresh)
• Dark mode + HTTPS = full features
```

**Auteur** : Frederic Boussemart @RicFid (2026)

**Fichiers** :
```
index.html     (structure)
script.js      (100% JS vanilla)
style.css      (CSS variables + dark)
manifest.json  (PWA)
assets/        (logo + backgrounds)
```

**Dépendances CDN** :
```
XLSX.js    (Excel)
Tesseract  (OCR)
FontAwesome
html-docx  (Word)
```

---

**Copié dans TODO-DESCRIPTION.md pour réutilisation !** ✅
