# 🚀 Instructions de Déploiement sur GitHub

## Étape 1 : Créer un Repository GitHub

1. Allez sur https://github.com
2. Cliquez sur le bouton **"New"** (ou le **+** en haut à droite > "New repository")
3. Remplissez les informations :
   - **Repository name** : `nutripure-commissions` (ou le nom de votre choix)
   - **Description** : "Application de gestion des commissions des coachs NutriPure"
   - Choisissez **Public** (pour GitHub Pages gratuit) ou **Private**
   - ✅ Cochez "Add a README file" (ou pas, on en a déjà un)
4. Cliquez sur **"Create repository"**

## Étape 2 : Initialiser Git localement

Ouvrez un terminal dans le dossier du projet et exécutez :

```bash
# Initialiser le repository Git
git init

# Ajouter tous les fichiers
git add .

# Créer le premier commit
git commit -m "🎉 Initial commit - Application NutriPure Commissions"

# Renommer la branche en main (si nécessaire)
git branch -M main

# Lier votre repository local au repository GitHub
git remote add origin https://github.com/VOTRE-USERNAME/nutripure-commissions.git

# Pousser le code sur GitHub
git push -u origin main
```

**Remplacez** `VOTRE-USERNAME` par votre nom d'utilisateur GitHub !

## Étape 3 : Activer GitHub Pages

1. Sur votre repository GitHub, allez dans **Settings** (⚙️)
2. Dans le menu de gauche, cliquez sur **Pages**
3. Dans la section "Build and deployment" :
   - **Source** : Sélectionnez "Deploy from a branch"
   - **Branch** : Sélectionnez `main` et `/root`
4. Cliquez sur **Save**

✅ Votre site sera disponible en quelques minutes à :
```
https://VOTRE-USERNAME.github.io/nutripure-commissions/
```

## Étape 4 : Mises à jour futures

Pour mettre à jour l'application après des modifications :

```bash
# Ajouter les modifications
git add .

# Créer un commit avec un message descriptif
git commit -m "✨ Ajout de nouvelles fonctionnalités"

# Pousser les modifications
git push
```

Les changements seront automatiquement déployés sur GitHub Pages !

## 📋 Checklist Rapide

- [ ] Repository GitHub créé
- [ ] Git initialisé localement
- [ ] Code poussé sur GitHub
- [ ] GitHub Pages activé
- [ ] Site accessible en ligne

## 🆘 En cas de problème

### Erreur "remote origin already exists"
```bash
git remote remove origin
git remote add origin https://github.com/VOTRE-USERNAME/nutripure-commissions.git
```

### Erreur "failed to push"
```bash
git pull origin main --rebase
git push -u origin main
```

### GitHub Pages ne fonctionne pas
- Vérifiez que le repository est public (ou que vous avez un plan GitHub Pro)
- Attendez 5-10 minutes après l'activation
- Vérifiez dans Settings > Pages que tout est bien configuré

## 🎯 Alternative : Déploiement sur d'autres plateformes

### Netlify (Gratuit)
1. Glissez-déposez le dossier sur https://app.netlify.com/drop
2. C'est tout ! 🎉

### Vercel (Gratuit)
1. Importez votre repository GitHub sur https://vercel.com
2. Déployez automatiquement

---

Besoin d'aide ? Contactez un développeur de l'équipe ! 💪
