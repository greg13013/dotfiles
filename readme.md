# 💻 My Dotfiles - Zsh & Zinit Configuration

Ce dépôt contient ma configuration personnelle pour **Zsh**, propulsée par **Zinit** pour la rapidité et **Powerlevel10k** pour l'interface visuelle.

## 🚀 Installation Rapide

Pour réinstaller cette configuration sur un nouvel environnement Ubuntu / WSL, suis ces étapes :

### 1. Mise à jour du système et dépendances
Copie et colle cette commande pour installer les outils de base nécessaires :

```bash
sudo apt update && sudo apt install git curl zsh fzf zoxide -y
```

### 2. Récupérer les fichiers
Clone ce dépôt dans ton dossier personnel :

```bash
git clone https://github.com/greg13013/dotfiles.git ~/dotfiles
```

### 3. Créer les liens symboliques
Ces commandes connectent ton système aux fichiers du dépôt (écrase les fichiers par défaut) :

```bash
ln -sf ~/dotfiles/zshrc ~/.zshrc
ln -sf ~/dotfiles/p10k.zsh ~/.p10k.zsh
```

### 4. Activer Zsh par défaut
Change ton shell pour que Zsh se lance au démarrage du terminal :

```bash
chsh -s $(which zsh)
```

## 🛠️ Outils inclus dans cette config

| Outil | Description |
| :--- | :--- |
| **Zinit** | Gestionnaire de plugins ultra-rapide. |
| **Powerlevel10k** | Thème de prompt ultra personnalisable. |
| **zsh-autosuggestions** | Propose la suite des commandes en gris clair. |
| **zsh-syntax-highlighting** | Colore les commandes (vert si ok, rouge si erreur). |
| **zoxide** | Le `cd` intelligent qui retient tes dossiers fréquents. |
| **fzf-tab** | Menu de sélection visuel pour la touche Tab. |

## ⚠️ Configuration visuelle (Important)
Pour que le thème s'affiche correctement (icônes, flèches, logos), tu **dois** installer une **Nerd Font** sur ton Windows et l'activer dans les paramètres de Windows Terminal.

* **Police recommandée :** `MesloLGS NF` ou `JetBrainsMono Nerd Font`.

## 🔄 Synchronisation
Si tu modifies ta configuration :
```bash
cd ~/dotfiles
git add .
git commit -m "Mise à jour de la config"
git push
```

Pour récupérer les changements sur une autre machine :
```bash
cd ~/dotfiles && git pull
```