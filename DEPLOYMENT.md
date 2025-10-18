# 🚀 Guide de Déploiement - AlphaPDF Legal Site

## 📦 Contenu du site

### Structure complète
```
alphapdf-legal-site/
├── index.html                      # Page d'accueil avec liens FR/EN
├── fr/                             # Pages françaises
│   ├── privacy_policy.html         # ← IMPORTANT pour Google Play
│   ├── terms_conditions.html
│   ├── mentions_legales.html
│   └── tarifs.html
├── en/                             # Pages anglaises
│   ├── privacy_policy.html
│   ├── terms_conditions.html
│   ├── legal_notice.html
│   └── pricing.html
├── assets/
│   ├── css/
│   │   └── style.css               # Styles responsive + dark mode auto
│   └── img/
│       └── favicon.svg             # Icône PDF rouge
├── robots.txt                      # SEO (Allow all)
├── sitemap.xml                     # Plan du site (9 URLs)
├── 404.html                        # Page erreur
├── README.md                       # Documentation
└── .gitignore                      # Fichiers à ignorer
```

**TOTAL : 14 fichiers**

---

## 🌐 Étapes de déploiement sur GitHub Pages

### Méthode 1 : Interface Web GitHub (RECOMMANDÉ)

1. **Créer un repository GitHub**
   - Allez sur https://github.com/new
   - Nom du repo : `alphapdf-legal` (ou autre nom)
   - Public ou Private (GitHub Pages fonctionne avec les deux)
   - Ne pas cocher "Initialize with README" (on a déjà nos fichiers)
   - Cliquez **Create repository**

2. **Uploader les fichiers**
   - Sur la page du repository, cliquez **Add file** → **Upload files**
   - Glissez-déposez TOUS les fichiers/dossiers de `alphapdf-legal-site/`
   - Message du commit : "Initial commit - AlphaPDF legal site"
   - Cliquez **Commit changes**

3. **Activer GitHub Pages**
   - Allez dans **Settings** (onglet en haut)
   - Dans le menu latéral, cliquez **Pages** (section "Code and automation")
   - Source : **Deploy from a branch**
   - Branch : **main** (ou master)
   - Folder : **/ (root)**
   - Cliquez **Save**

4. **Attendre le déploiement**
   - GitHub va construire le site (1-3 minutes)
   - Une fois prêt, l'URL apparaîtra en haut : 
     `https://yourusername.github.io/alphapdf-legal/`
   - Cliquez sur l'URL pour vérifier

5. **Personnaliser l'URL (optionnel)**
   - Dans Pages → Custom domain (si vous avez un domaine)
   - Sinon, utilisez l'URL GitHub directement

---

### Méthode 2 : Git CLI (pour utilisateurs avancés)

```bash
# Dans le dossier alphapdf-legal-site/
git init
git add .
git commit -m "Initial commit - AlphaPDF legal site"
git branch -M main
git remote add origin https://github.com/VOTRE_USERNAME/alphapdf-legal.git
git push -u origin main
```

Puis activez Pages dans Settings comme décrit ci-dessus.

---

## 📱 Intégration dans Google Play Console

### Lien requis pour Google Play

Lors de la soumission de votre app sur Google Play Console, utilisez cette URL pour le champ **"Politique de confidentialité"** :

```
https://VOTRE_USERNAME.github.io/alphapdf-legal/fr/privacy_policy.html
```

**⚠️ IMPORTANT** : Remplacez `VOTRE_USERNAME` par votre nom d'utilisateur GitHub réel.

### Exemple concret
Si votre username GitHub est `dadamine86`, l'URL sera :
```
https://dadamine86.github.io/alphapdf-legal/fr/privacy_policy.html
```

### Où mettre ce lien dans Google Play Console

1. **Console Play** → Votre application
2. **Contenu de l'application** → **Confidentialité de l'app**
3. **Politique de confidentialité** → Collez l'URL
4. **Enregistrer**

---

## 🎨 Personnalisation post-déploiement

### 1. Mettre à jour l'URL dans robots.txt et sitemap.xml

Remplacez `yourusername.github.io/alphapdf-legal-site` par votre URL réelle :

**robots.txt :**
```
Sitemap: https://VOTRE_USERNAME.github.io/alphapdf-legal/sitemap.xml
```

**sitemap.xml :**
```xml
<loc>https://VOTRE_USERNAME.github.io/alphapdf-legal/</loc>
```
(Répétez pour toutes les 9 URLs)

### 2. Convertir favicon.svg en PNG (optionnel)

Le SVG fonctionne tel quel, mais pour une compatibilité maximale :

1. Ouvrez `assets/img/favicon.svg` dans un navigateur
2. Allez sur https://cloudconvert.com/svg-to-png
3. Uploadez le fichier, convertissez en PNG 64x64
4. Téléchargez et renommez en `favicon.png`
5. Placez dans `assets/img/favicon.png`
6. Modifiez les `<link rel="icon"...>` dans tous les HTML :
   ```html
   <link rel="icon" type="image/png" href="../assets/img/favicon.png">
   ```

---

## ✅ Vérification des liens

Tous les liens ont été testés et fonctionnent :

### Navigation interne (index.html)
- ✅ Liens vers 4 pages FR
- ✅ Liens vers 4 pages EN
- ✅ Ancres #fr et #en

### Navigation header (chaque page)
- ✅ Retour accueil (../index.html ou index.html)
- ✅ Navigation entre pages du même langage

### Footer
- ✅ Email : `mailto:dadamine86@gmail.com`
- ✅ Site officiel : `https://sites.google.com/view/aminetelecom/accueil`

### Page 404
- ✅ Retour accueil
- ✅ Liens vers toutes les pages

---

## 📊 Statistiques

- **Pages HTML** : 9 (index + 4 FR + 4 EN)
- **Fichiers CSS** : 1 (responsive + dark mode auto)
- **Fichiers config** : 3 (robots.txt, sitemap.xml, .gitignore)
- **Documentation** : 2 (README.md, DEPLOYMENT.md)
- **Total** : 16 fichiers

**Poids total** : < 200 KB

---

## 🔒 Sécurité

- ✅ Pas de JavaScript externe (CDN)
- ✅ Pas de tracking/analytics
- ✅ Pas de cookies
- ✅ HTTPS uniquement (GitHub Pages force HTTPS)
- ✅ Responsive mobile-first
- ✅ Accessible (semantic HTML, headings, alt texts)

---

## 📞 Support

Pour toute question :
- **Email** : dadamine86@gmail.com
- **Site** : https://sites.google.com/view/aminetelecom/accueil

---

© 2025 Amine Telecom — Noeva Labs

