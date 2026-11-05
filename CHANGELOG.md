# Nouveautés de Navis

Chaque version publiée a sa section ci-dessous ; le script `Publier.bat` reprend la section de la version
pour les notes de la release GitHub et la page publique.

## 0.3.0 — 4 novembre 2026

Première version publique.

### Explorer
- Vue **Détails** rapide (dossiers de plus de 5 000 éléments affichés en moins d'une seconde), tri naturel (`fichier2` avant `fichier10`), dossiers en premier.
- **Dossiers dépliables sur place** : flèche ▸ / ▾, Alt+clic pour tout déplier (5 niveaux), Ctrl+Alt+Gauche pour tout replier ; l'état déplié est gardé dans l'historique.
- **Vue en colonnes** façon Finder (Ctrl+Maj+L).
- **Taille des dossiers** calculée en arrière-plan.
- **Panneau latéral** (F8) : accès rapide, dossiers épinglés (Ctrl+D), tous les lecteurs avec leur espace libre.

### Aperçus
- **Panneau d'aperçu** (F7) : images, texte et code, PDF, Word / Excel / PowerPoint, modèles 3D STL et OBJ ; chaque type peut être désactivé.
- **Aperçu rapide** avec la barre Espace, animation de zoom façon macOS.

### Fichiers
- Clic droit : actions de base, et le **vrai menu Windows** (7-Zip, Git, Envoyer vers…).
- Couper / copier / coller compatibles avec l'Explorateur, Corbeille, renommage sur place (F2), nouveau dossier (Ctrl+Maj+N).
- Mise à jour automatique quand un fichier change.

### Recherche
- **Recherche** dans le dossier courant et ses sous-dossiers (Ctrl+F) : `*.exe`, `*.(png|jpg)`, mots, `~exclure`, `regex:`, `type:dossier`, `taille:>100mo`, `date:<7j`…
- **Index de recherche** : résultats en moins d'un quart de seconde sur tout un disque, mis à jour en direct (menu Outils > Index de recherche).
