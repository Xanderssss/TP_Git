# 🌟 TP3 GIT

## 📌 Étape I : Création et Initialisation d'un Nouveau Dépôt

### 📁 Création du dépôt
```bash
$ cd xcs310
$ mkdir tp3
$ cd tp3
$ git init
Initialized empty Git repository in C:/Users/Xander/xcs310/tp3/.git/
```

### 📄 Création du fichier `README.md`
```bash
$ nano README.md
```

### ✅ Premier commit
```bash
$ git add README.md
$ git commit -m "Premier commit : création du README"
```

---

## 🌿 Étape II : Gestion des branches et modifications

### 🌳 Création des branches
```bash
$ git branch featur-1
$ git branch feature-2
$ git branch
```

### 🔀 Changement vers la branche `featur-1`
```bash
$ git switch featur-1
```

### 🖊️ Modification du fichier `README.md`
```bash
$ echo "Modification dans feature-1" >> README.md
```

### 📦 Ajout et commit des modifications
```bash
$ git add README.md
$ git commit -m "Ajout de la ligne 'Modification dans feature-1' dans README.md"
```

### 🔄 Retour à la branche `main`
```bash
$ git switch main
```

### 📑 Vérification du fichier
```bash
$ cat README.md
```

---

## 🌱 Étape III : Création et Fusion d'une branche de développement

### 🌿 Création de la branche `dev`
```bash
$ git branch dev
```

### 📝 Création du fichier `notes.txt`
```bash
$ git switch dev
$ echo "Ceci est le contenu du fichier notes.txt" > notes.txt
```

### 📌 Commit du fichier `notes.txt`
```bash
$ git add notes.txt
$ git commit -m "Ajout du fichier notes.txt"
```

### 🔄 Fusion de la branche `dev` dans `main`
```bash
$ git switch main
$ git merge dev
```

### 📁 Vérification de la fusion
```bash
$ ls
```

### 🗑️ Suppression de la branche `dev`
```bash
$ git branch -d dev
```

---

