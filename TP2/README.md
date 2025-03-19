# 🚀 TP2 GIT

## 📌 Étape I : Création du Répertoire et Initialisation du Dépôt

### 📂 Création du répertoire `TP2`
```bash
$ mkdir tp2
$ cd tp2
```

### 📝 Création des fichiers nécessaires
```bash
$ nano operation.py
$ nano calc.py
```

### 🛠️ Initialisation du dépôt Git
```bash
$ git init
```

### 📌 Ajout et commit des fichiers
```bash
$ git add .
$ git commit -m "Initial commit"
```

### 🔎 Vérification de l'historique Git
```bash
$ git log
```

### 🏷️ Ajout d'un tag `v1.0`
```bash
$ git tag v1.0
```

---

## ✏️ Étape II : Modification et Nouveau Commit

### 📝 Modification des fichiers
```bash
$ nano operation.py
$ nano calc.py
```

### 📌 Ajout et commit des modifications
```bash
$ git add .
$ git commit -m "Ajout fonction divide"
```

### 📑 Vérification de l'historique
```bash
$ git log --oneline
```

---

## 🌳 Étape III : Historique condensé

Voici plusieurs façons pratiques de visualiser l’historique :

- Historique complet :
```bash
git log --all
```

- Historique décoré
```bash
git log --decorate
```

- Historique condensé
```bash
git log --oneline
```

- Historique graphique
```bash
git log --graph
```

### ⚙️ Création d'un alias Git utile
```bash
git config --global alias.adog "log --all --decorate --oneline --graph"
```

Utilisation :
```bash
git adog
```

---

## 🔧 Étape II : Gestion des Erreurs et Annulations

### 🌳 Création de branches pour corriger l'erreur
```bash
$ git branch fix-checkout
$ git branch fix-reset
$ git branch fix-revert
```

### 🔎 Vérification des branches
```bash
git adog
```

---

## 🔄 Étape V : Annuler avec `git checkout`

### 🔀 Sélection de la branche
```bash
$ git checkout fix-checkout
```

### ⏪ Annulation des modifications avec `checkout`
```bash
$ git checkout v1.0 calc.py operation.py
```

### 📝 Correction puis commit
```bash
$ nano operation.py
$ nano calc.py
$ git add .
$ git commit -m "Fix divide function with git checkout"
```

---

## 🔄 Étape VI : Annuler avec `git reset`

### 🔃 Annulation avec reset
```bash
$ git checkout fix-reset
$ git reset --hard HEAD~1
```

### 📝 Modification et commit
```bash
$ nano operation.py
$ nano calc.py
$ git add .
$ git commit -m "Fix divide function with git reset"
```

---

## 🔄 Étape VII : Annulation avec `git revert`

### 🔙 Annulation avec revert
```bash
$ git checkout fix-revert
$ git revert HEAD
```

### 📝 Modification puis commit
```bash
$ nano operation.py
$ nano calc.py
$ git add .
$ git commit -m "Fix divide function with git revert"
```

---

## 🌿 Étape VIII : Fusion des Corrections dans `main`

### 📥 Fusionner les corrections
```bash
$ git checkout main
$ git merge fix-revert
```

### 🏷️ Ajout d'un tag `v2.0`
```bash
$ git tag v2.0
```

---

## 🏁 Étape IX : Finalisation

### ✅ Vérification finale
```bash
$ git status
```

### 📌 Commit final des solutions
```bash
$ nano .gitignore
$ git add .gitignore reponses.md
$ git commit -m "Solution TP2"
```

---


