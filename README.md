🚀 Tech Commander v176 [PyAutoGUI Edition]
Tech Commander est un utilitaire d'administration système tout-en-un doté d'une interface graphique (GUI) développée en PowerShell. Il combine des outils de maintenance Windows, la génération de documents automatisée et l'intégration de l'intelligence artificielle en local pour générer et exécuter des macros de contrôle (souris/clavier) à la volée. 🪄

Ce projet utilise un lanceur hybride Batch/PowerShell (.bat qui lit et exécute son propre code PowerShell) pour contourner les restrictions d'exécution par défaut de Windows. 🛡️

✨ Fonctionnalités Principales
🤖 Contrôle IA Dynamique : Interface de prompt connectée à Ollama (llama3.1) pour traduire des requêtes en langage naturel en scripts Python (pyautogui), exécutés instantanément pour automatiser des actions sur l'ordinateur.

🔧 Maintenance Système : Outils intégrés pour nettoyer les fichiers temporaires, vérifier la santé des disques (SMART), sauvegarder les pilotes système et lancer des réparations via sfc /scannow.

🌐 Gestion Réseau : Raccourcis rapides pour réinitialiser la pile TCP/IP et le cache DNS, tester la connectivité (Ping) et gérer les cartes réseau.

💼 Outils Métier & Admin : Génération automatisée de devis via une intégration Microsoft Excel (COM object), activation du compte Super-Admin Windows et réparation du spooler d'impression.

📊 Monitoring en temps réel : Affichage de la charge CPU en direct et de l'utilisateur actif directement dans l'interface.

⚙️ Prérequis
Pour utiliser l'ensemble des fonctionnalités de Tech Commander, l'environnement suivant est requis :

🪟 OS : Windows 10 ou Windows 11.

🦙 Ollama : Installé localement avec le modèle llama3.1 téléchargé (ollama run llama3.1).

🐍 Python : Installé et ajouté au PATH, avec la bibliothèque PyAutoGUI (pip install pyautogui).

📊 Microsoft Excel : Requis uniquement pour la fonctionnalité de génération de devis.

📦 Winget : Requis pour l'installation automatisée du pack de logiciels (Chrome, VLC, etc.).

🚀 Installation et Utilisation
📥 Clonez ce dépôt sur votre machine locale.

✅ Assurez-vous que les prérequis (Python, Ollama) sont lancés et fonctionnels.

▶️ Double-cliquez simplement sur le fichier .bat.

🔓 Le script s'occupe de contourner les politiques d'exécution PowerShell (ExecutionPolicy Bypass) et lance l'interface graphique "Neural Commander".

🏗️ Architecture du Script
📜 Lanceur Batch : Sécurise le lancement, garde la console ouverte en cas de crash pour le débogage, et passe le relais à PowerShell.

🖥️ Interface Windows Forms : Créée dynamiquement via PowerShell, sans dépendre d'outils tiers de création d'UI.

⚙️ Générateur Python : Filtre les réponses d'Ollama pour extraire le code pur, crée un fichier temporaire .py et l'exécute dans un processus distinct sécurisé.
