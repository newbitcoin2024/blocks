
# 🚀 Accelerate NewBitcoin Blockchain Synchronization  

This guide explains how to download and directly add the blockchain blocks to speed up the synchronization of your Bitcoin Core client.  

## 📌 Prerequisites  
- Have **NewBitcoin-Core** installed on your computer.  
- Have **enough disk space** to store the blockchain.  
- Have **Git** installed on your system.  

## 🛠️ Instructions  

### 1️⃣ Install Bitcoin Core  
- Download **Bitcoin Core** from the official website or compile it from the source code.  
- Run Bitcoin Core once so it generates the configuration folders.  
- **Close Bitcoin Core** before proceeding to the next steps.  

### 2️⃣ Download the blocks folder  
- Open a terminal and run the following command to clone the repository containing the blockchain blocks:  
  ```sh
  git clone https://github.com/newbitcoin2024/blocks.git
  ```  

### 3️⃣ Copy the blocks to the Bitcoin folder  
- Locate the Bitcoin Core data folder:  
  - **Windows**: `%APPDATA%\Bitcoin\`  
  - **Linux**: `~/.bitcoin/`  
  - **macOS**: `~/Library/Application Support/Bitcoin/`  
- Copy the contents of the downloaded `blocks` folder into the Bitcoin Core folder:  
  ```sh
  cp -r blocks/* ~/.bitcoin/blocks/
  ```  

### 4️⃣ Restart Bitcoin Core  
- **Open Bitcoin Core**. It should detect the copied blocks and synchronize the remaining data much faster.  

## ⚠️ Note  
Using external block files can **significantly reduce synchronization time**, but always ensure the authenticity of the downloaded files.  

---

En Francaise

# Accélérer la synchronisation de la blockchain NewBitcoin

Ce guide explique comment télécharger et ajouter directement les blocs de la blockchain NewBitcoin afin d'accélérer la synchronisation de votre client Bitcoin Core.

## Prérequis
- Avoir installé NewBitcoin-Core sur votre ordinateur.
- Disposer d'un espace disque suffisant pour stocker la blockchain.
- Avoir git installé sur votre système.

## Instructions

1. **Installer Bitcoin Core**
   - Téléchargez Bitcoin Core depuis le site officiel ou compilez-le à partir du code source.
   - Lancez Bitcoin Core une première fois pour qu'il génère les dossiers de configuration.
   - Fermez Bitcoin Core avant de procéder aux étapes suivantes.

2. **Télécharger le dossier des blocs**
   - Ouvrez un terminal et exécutez la commande suivante pour cloner le référentiel contenant les blocs :
     ```sh
     git clone https://github.com/newbitcoin2024/blocks.git
     ```

3. **Copier les blocs dans le dossier Bitcoin**
   - Trouvez le dossier de données de Bitcoin Core :
     - Sous Windows : `%APPDATA%\Bitcoin\`
     - Sous Linux : `~/.bitcoin/`
     - Sous macOS : `~/Library/Application Support/Bitcoin/`
   - Copiez le contenu du dossier `blocks` téléchargé dans ce dossier.
     ```sh
     cp -r blocks/* ~/.bitcoin/blocks/
     ```

4. **Relancer Bitcoin Core**
   - Ouvrez Bitcoin Core. Il devrait détecter les blocs copiés et synchroniser le reste beaucoup plus rapidement.

## Remarque
L'utilisation de fichiers blocs externes peut réduire le temps de synchronisation, mais vérifiez toujours l'authenticité des fichiers téléchargés.

---

Pour plus d'informations, consultez le référentiel officiel : [NewBitcoin Blocks Repository](https://github.com/newbitcoin2024/blocks.git).

