# Carnet de recettes

Un carnet de recettes qui fonctionne dans **Claude** (claude.ai).

Colle une recette en vrac, une capture d'écran ou une photo d'une page de livre, et Claude en fait une fiche toujours dans le même format :

- titre, catégorie (poulet, bœuf, porc, poisson, pâtes, végé, desserts…) et mots clés;
- liste d'ingrédients, avec les petites quantités en c. à thé et c. à table;
- étapes détaillées qui reprennent les quantités de chaque ingrédient;
- programme pour le thermomètre **Meater** quand c'est de la viande ou du poisson (températures de Santé Canada);
- photo du plat : la tienne, celle trouvée dans ta capture, ou une illustration dessinée par Claude.

Tu peux modifier chaque fiche, chercher par ingrédient ou mot clé, et trier par catégorie. Sur cellulaire, tu peux prendre une photo directement. Chaque fiche est aussi copiée automatiquement en document Google Docs dans ton Google Drive, dans un dossier « Carnet de recettes ».

## Installation

Le carnet a besoin de Claude pour fonctionner : il ne marche pas si on ouvre le fichier directement ou avec GitHub Pages. Chaque personne l'installe dans son propre compte Claude, et ses recettes restent privées.

1. Télécharge le fichier [`carnet-recettes.html`](carnet-recettes.html).
2. Ouvre une nouvelle conversation sur [claude.ai](https://claude.ai) et joins-y le fichier.
3. Copie-colle ce message :

   > Publie ce fichier comme artefact, tel quel, avec ces capacités : db avec la règle {path: "recettes", read: "view", write: "admin"}, sample avec images: true, assets, downloads, et mcp avec le serveur "Google Drive" et les outils search_files, create_file et trash_file.

4. Pour la sauvegarde dans Google Drive, connecte Google Drive dans les paramètres de Claude, sous Connecteurs. Sans Drive, tout le reste fonctionne.
5. Pour l'avoir sur ton cellulaire, ouvre le lien du carnet dans Safari ou Chrome et choisis « Ajouter à l'écran d'accueil ».

À la première utilisation, le carnet te demande d'autoriser Claude (pour analyser les recettes) et Google Drive. L'analyse compte dans ton utilisation de Claude.

## Sauvegarde

- **Automatique** : un document Google Docs par recette, dans le dossier Drive « Carnet de recettes ».
- **Manuelle** : le bouton *Exporter* crée un fichier JSON avec toutes les recettes; *Importer* le recharge.
