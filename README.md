# 🏆 GitHub Achievements & Trophies Farm

Ce projet contient tout ce dont vous avez besoin pour débloquer le maximum de **badges officiels GitHub** et afficher vos **trophées de profil**.

---

## 🎖️ 1. Badges Officiels GitHub Débloquables

| Badge | Nom | Condition | Méthode d'obtention |
|---|---|---|---|
| ⚡ | **Quickdraw** | Fermer une Issue ou PR en moins de 5 minutes | Automatisé par le script |
| 🪂 | **YOLO** | Fusionner une Pull Request sans code review | Automatisé par le script |
| 👯 | **Pair Extraordinaire** | Avoir un commit co-écrit (`Co-authored-by`) dans une PR fusionnée | Automatisé par le script |
| 🦈 | **Pull Shark** (x1, x16, x128) | Fusionner 1, 16 ou 128 Pull Requests | Automatisé par le script |
| 🧠 | **Galaxy Brain** (x2, x8, x16, x32) | Avoir des réponses acceptées dans des Discussions GitHub | Manuel (Section dédiée ci-dessous) |
| 💖 | **Public Sponsor** | Sponsoriser un projet ou créateur via GitHub Sponsors | Faire un don (\$1) sur GitHub Sponsors |
| 🌟 | **Starstruck** (16, 128, 512...) | Obtenir des étoiles sur vos dépôts publics | Nécessite des vraies étoiles d'utilisateurs |

> **Note importante** : Les succès GitHub ne se débloquent que sur des **dépôts publics**.

---

## 🚀 2. Méthode 1 (Recommandée) : GitHub Actions (100% Automatique dans le Cloud)

Vous n'avez même pas besoin d'installer de clés ou d'outils en local.

1. Créez un nouveau dépôt public sur GitHub : [https://github.com/new](https://github.com/new)
   - Nommez-le par exemple `github-achievements-farmer`.
   - Cochez **Public**.
2. Envoyez ce dossier sur ce dépôt :
   ```bash
   git init
   git add .
   git commit -m "feat: setup achievements farmer"
   git branch -M main
   git remote add origin https://github.com/<VOTRE_PSEUDO>/github-achievements-farmer.git
   git push -u origin main
   ```
3. Sur GitHub, activez les permissions d'écriture pour les Actions :
   - Allez dans **Settings** du dépôt > **Actions** > **General**.
   - Dans **Workflow permissions**, cochez **Read and write permissions**.
   - Cochez **Allow GitHub Actions to create and approve pull requests**.
   - Cliquez sur **Save**.
4. Lancez le workflow :
   - Allez dans l'onglet **Actions** de votre dépôt.
   - Cliquez sur **Farm GitHub Achievements** à gauche.
   - Cliquez sur **Run workflow** (choisissez 16 ou 128 PRs).
   - En quelques minutes, vos succès **Quickdraw**, **YOLO**, **Pair Extraordinaire** et **Pull Shark** seront débloqués !

---

## 🐍 3. Méthode 2 : Exécution Locale avec le Script Python

Si vous préférez exécuter le script directement sur votre machine :

1. Générez un token GitHub classique (PAT) avec la permission `repo` :
   - [https://github.com/settings/tokens/new](https://github.com/settings/tokens/new)
2. Installez `requests` si nécessaire :
   ```bash
   pip3 install requests
   ```
3. Lancez le farm :
   ```bash
   python3 farmer.py <VOTRE_TOKEN_GITHUB> 16
   ```
   *(Remplacez 16 par 128 si vous voulez directement le Pull Shark Gold)*.

---

## 🧠 4. Comment obtenir le badge "Galaxy Brain" (Discussions)

Pour débloquer **Galaxy Brain** (cerveau de galaxie) :
1. Sur un de vos dépôts publics, allez dans **Settings** > activez **Discussions**.
2. Créez une discussion dans la catégorie **Q&A**.
3. Posez une question (ou demandez à un ami / second compte de poser une question).
4. Répondez à la question avec votre compte.
5. Marquez votre réponse comme **Answer** (Réponse acceptée).
   - Niveau 1 : 2 réponses acceptées
   - Niveau 2 : 8 réponses acceptées
   - Niveau 3 : 16 réponses acceptées
   - Niveau 4 : 32 réponses acceptées

---

## 🏆 5. Trophées de Profil (Widget `github-profile-trophy`)

Si vous voulez afficher la vitrine de trophées animés sur votre profil GitHub :

Ajoutez ceci dans le `README.md` de votre profil spécial (`https://github.com/<VOTRE_PSEUDO>/<VOTRE_PSEUDO>`) :

```markdown
[![trophy](https://github-profile-trophy.vercel.app/?username=VOTRE_PSEUDO&theme=onedark)](https://github.com/ryo-ma/github-profile-trophy)
```
*(Remplacez `VOTRE_PSEUDO` par votre nom d'utilisateur GitHub)*.
