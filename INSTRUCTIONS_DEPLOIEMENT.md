# 🚀 INSTRUCTIONS DE DÉPLOIEMENT — AlphaPDF Legal Site

## ✅ Site créé le : 18 octobre 2025

---

## 📦 CONTENU DU SITE

### **Structure complète (17 fichiers) :**

```
alphapdf-legal-site/
├── index.html                          ✅ Page d'accueil FR/EN
├── fr/                                 ✅ 4 pages françaises
│   ├── privacy_policy.html            ⭐ IMPORTANT pour Google Play
│   ├── terms_conditions.html
│   ├── mentions_legales.html
│   └── tarifs.html
├── en/                                 ✅ 4 pages anglaises
│   ├── privacy_policy.html
│   ├── terms_conditions.html
│   ├── legal_notice.html
│   └── pricing.html
├── assets/
│   ├── css/style.css                  ✅ Responsive + dark mode
│   └── img/favicon.svg                ✅ Logo PDF rouge
├── robots.txt                          ✅ SEO
├── sitemap.xml                         ✅ 9 URLs
├── 404.html                            ✅ Page erreur
├── README.md                           ✅ Documentation
├── DEPLOYMENT.md                       ✅ Guide technique
└── INSTRUCTIONS_DEPLOIEMENT.md        ✅ Ce fichier
```

---

## 🌐 DÉPLOIEMENT GITHUB PAGES (5 MINUTES)

### **Étape 1 : Créer le repository**

1. Allez sur : https://github.com/new
2. Repository name : `alphapdf-privacy`
3. Description : "Legal pages for AlphaPDF - Noeva Labs"
4. Visibilité : **Public** ✅
5. Ne cochez RIEN d'autre (pas de README, pas de .gitignore)
6. Cliquez **Create repository**

---

### **Étape 2 : Uploader tous les fichiers**

**Option A : Interface Web (RECOMMANDÉ)**

1. Sur la page du repository vide, cliquez sur **uploading an existing file**
2. Glissez-déposez **TOUS les fichiers et dossiers** de `alphapdf-legal-site/` :
   - index.html
   - Dossiers : fr/, en/, assets/
   - Fichiers : robots.txt, sitemap.xml, 404.html, README.md, etc.
3. Commit message : `Initial commit - AlphaPDF legal site`
4. Cliquez **Commit changes**

**Option B : Git CLI**

```bash
cd alphapdf-legal-site
git init
git add .
git commit -m "Initial commit - AlphaPDF legal site"
git branch -M main
git remote add origin https://github.com/dadamine86-commits/alphapdf-privacy.git
git push -u origin main
```

---

### **Étape 3 : Activer GitHub Pages**

1. Dans le repository, cliquez sur **Settings** (onglet en haut)
2. Menu latéral gauche → **Pages** (section "Code and automation")
3. Source : **Deploy from a branch**
4. Branch : **main** ✅
5. Folder : **/ (root)** ✅
6. Cliquez **Save**
7. **Attendez 2-3 minutes** ⏱️

Une bannière verte apparaîtra avec le message :
```
✅ Your site is live at https://dadamine86-commits.github.io/alphapdf-privacy/
```

---

## 🔗 URLS FINALES (Après déploiement)

### **Site principal :**
```
https://dadamine86-commits.github.io/alphapdf-privacy/
```

### **🇫🇷 Pages françaises :**
- **Privacy (RGPD)** : `https://dadamine86-commits.github.io/alphapdf-privacy/fr/privacy_policy.html` ⭐
- **CGU** : `https://dadamine86-commits.github.io/alphapdf-privacy/fr/terms_conditions.html`
- **Mentions** : `https://dadamine86-commits.github.io/alphapdf-privacy/fr/mentions_legales.html`
- **Tarifs** : `https://dadamine86-commits.github.io/alphapdf-privacy/fr/tarifs.html`

### **🇬🇧 Pages anglaises :**
- **Privacy** : `https://dadamine86-commits.github.io/alphapdf-privacy/en/privacy_policy.html`
- **Terms** : `https://dadamine86-commits.github.io/alphapdf-privacy/en/terms_conditions.html`
- **Legal** : `https://dadamine86-commits.github.io/alphapdf-privacy/en/legal_notice.html`
- **Pricing** : `https://dadamine86-commits.github.io/alphapdf-privacy/en/pricing.html`

---

## 📱 INTÉGRATION GOOGLE PLAY CONSOLE

### **URL à fournir dans Play Console :**

```
https://dadamine86-commits.github.io/alphapdf-privacy/fr/privacy_policy.html
```

### **Où la mettre :**

1. **Google Play Console** → Votre application AlphaPDF
2. Menu gauche → **Contenu de l'application**
3. **Confidentialité de l'app**
4. Champ **"URL de la politique de confidentialité"**
5. Collez : `https://dadamine86-commits.github.io/alphapdf-privacy/fr/privacy_policy.html`
6. Cliquez **Enregistrer**

✅ **Google Play acceptera cette URL** (conforme RGPD, contenu complet)

---

## ✅ VÉRIFICATION POST-DÉPLOIEMENT

### **1. Tester tous les liens (5 min)**

Ouvrez `https://dadamine86-commits.github.io/alphapdf-privacy/` et cliquez sur :
- ✅ Chaque lien de l'accueil (4 FR + 4 EN)
- ✅ Navigation header (Accueil, Privacy, Terms, etc.)
- ✅ Liens footer (email, site officiel)
- ✅ Liens internes dans les pages (renvois entre pages)

**Aucun lien ne doit renvoyer 404**

### **2. Tester responsive**

- Ouvrez sur mobile / tablette / desktop
- Vérifiez que la navigation fonctionne
- Testez le dark mode (si votre système est en mode sombre)

### **3. Tester 404**

Tapez une URL inexistante :
```
https://dadamine86-commits.github.io/alphapdf-privacy/page-qui-nexiste-pas
```

Doit afficher votre page 404 personnalisée avec lien retour accueil

---

## 📋 INFORMATIONS PRÉSENTES SUR TOUTES LES PAGES

- ✅ **Marque** : Noeva Labs
- ✅ **Éditeur légal** : Amine Telecom — Amine Lalouani
- ✅ **SIRET** : 81036711000014
- ✅ **Adresse** : 89B Grande Rue, 59100 Roubaix, France
- ✅ **Email** : dadamine86@gmail.com
- ✅ **Site officiel** : https://sites.google.com/view/aminetelecom/accueil
- ✅ **Date** : 18/10/2025 (FR) ou October 18, 2025 (EN)

### **Spécifications techniques :**
- ✅ Âge minimum : 16 ans (RGPD mineurs)
- ✅ Paiement : Google Play uniquement
- ✅ Litiges : Tribunal de Lille
- ✅ Licence : Usage non commercial uniquement
- ✅ IA locale : 100% offline, aucune donnée transmise
- ✅ Pub récompense : 60s vidéo → 1h accès complet

---

## 🎨 FEATURES DU SITE

- ✅ **Responsive** : Mobile-first, adaptatif
- ✅ **Dark mode auto** : `prefers-color-scheme: dark`
- ✅ **Navigation complète** : Header + Footer sur chaque page
- ✅ **Tous liens internes vérifiés** : Aucun 404
- ✅ **SEO** : Meta tags, sitemap.xml, robots.txt
- ✅ **Accessible** : Semantic HTML, contrastes OK
- ✅ **Léger** : < 200 KB total, aucune dépendance
- ✅ **Pur HTML/CSS** : Pas de framework, pas de build

---

## 📝 CHECKLIST FINALE

| Élément | Statut |
|---------|--------|
| ✅ 8 pages HTML (4 FR + 4 EN) | ✅ CRÉÉS |
| ✅ index.html avec navigation | ✅ CRÉÉ |
| ✅ style.css responsive + dark mode | ✅ CRÉÉ |
| ✅ favicon.svg (PDF rouge) | ✅ CRÉÉ |
| ✅ robots.txt avec vraie URL | ✅ CRÉÉ |
| ✅ sitemap.xml avec 9 URLs | ✅ CRÉÉ |
| ✅ 404.html personnalisé | ✅ CRÉÉ |
| ✅ README.md avec liens réels | ✅ CRÉÉ |
| ✅ Tous liens internes fonctionnels | ✅ VÉRIFIÉ |
| ✅ Mentions légales complètes | ✅ VÉRIFIÉ |
| ✅ RGPD conforme (IA locale) | ✅ VÉRIFIÉ |
| ✅ Paiement Google Play | ✅ CORRIGÉ |
| ✅ Âge minimum 16 ans | ✅ VÉRIFIÉ |
| ✅ Tribunal de Lille | ✅ VÉRIFIÉ |

---

## 🎯 PROCHAINE ÉTAPE

**Uploadez le contenu de `alphapdf-legal-site/` sur GitHub maintenant !**

Le site sera disponible en 2-3 minutes à :
```
https://dadamine86-commits.github.io/alphapdf-privacy/
```

---

**Créé le :** 18 octobre 2025  
**Par :** Cursor AI  
**Pour :** AlphaPDF / Noeva Labs  
**Statut :** ✅ **100% PRÊT À DÉPLOYER**

