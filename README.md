# eBooks Landing Page - GitHub Pages

Cette landing page statique capture les clics de campagne et redirige vers l'app mobile eBooks.

## 🚀 Déploiement GitHub Pages

### 1. Créer le Repository
```bash
# Créer un nouveau repository sur GitHub nommé 'ebooks-landing'
# Puis cloner et ajouter les fichiers
git clone https://github.com/VOTRE-USERNAME/ebooks-landing.git
cd ebooks-landing
```

### 2. Ajouter les Fichiers
- Copier `index.html` dans le repository
- Commit et push

### 3. Activer GitHub Pages
1. Aller dans Settings > Pages
2. Source: Deploy from a branch
3. Branch: main / (root)
4. Save

### 4. Configuration
Votre landing page sera accessible à: `https://VOTRE-USERNAME.github.io/ebooks-landing`

## ⚙️ Configuration Required

### Dans le fichier `index.html`:
Remplacez ces valeurs:
```javascript
const SUPABASE_URL = 'VOTRE_SUPABASE_URL';
const SUPABASE_ANON_KEY = 'VOTRE_SUPABASE_ANON_KEY';
```

### Dans le panel web (`CampaignLinksPage.jsx`):
Remplacez:
```javascript
'https://votre-username.github.io/ebooks-landing'
```
Par votre vraie URL GitHub Pages.

## 🧪 Test de Fonctionnement

1. **Créer un lien de campagne** dans le panel web
2. **Cliquer sur le lien** → Landing page s'affiche
3. **Vérifier le deep link** → Tentative d'ouverture de l'app
4. **Fallback Play Store** → Redirection si app pas installée

## 📱 URLs de Test

### Format généré:
```
https://VOTRE-USERNAME.github.io/ebooks-landing?utm_source=tiktok&utm_campaign=test&ebook_id=123&campaign_id=456&deep_link=true
```

### Deep Link généré:
```
ebooks://?utm_source=tiktok&utm_campaign=test&ebook_id=123&campaign_id=456
```

## 🔧 Fonctionnalités

- ✅ Tracking des clics en base Supabase
- ✅ Affichage du livre d'appel (si configuré)
- ✅ Tentative d'ouverture automatique de l'app
- ✅ Fallback vers Play Store
- ✅ Design responsive et moderne
- ✅ Compatible tous navigateurs

## 📊 Analytics Capturées

- Device type (mobile/desktop)
- Browser & OS
- Referrer URL
- User Agent
- Timestamp du clic

---

**Note**: Cette solution est gratuite, fiable et ne nécessite aucun serveur backend !