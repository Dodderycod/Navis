# Nouveautés de Navis

Chaque version publiée a sa section ci-dessous ; le script `Publier.bat` reprend la section de la version
pour les notes de la release GitHub et la page publique.

## 0.5.0 — 12 novembre 2026

### Onglets
- **Plusieurs onglets** par volet, chacun avec son dossier et son historique Précédent / Suivant.
- **Ctrl+T** nouvel onglet, **Ctrl+W** fermer, **Ctrl+Maj+T** rouvrir le dernier onglet fermé, **Ctrl+Tab** / **Ctrl+Maj+Tab** onglet suivant / précédent.
- **Clic du milieu** sur un dossier : il s'ouvre dans un nouvel onglet. Clic du milieu sur un onglet : il se ferme. Double-clic dans la barre d'onglets : nouvel onglet.
- Glisser un onglet pour le réordonner ou le mettre dans un autre volet. Clic droit : dupliquer, fermer les autres, fermer ceux de droite, déplacer dans un nouveau volet.
- En changeant d'onglet, la sélection et le défilement sont retrouvés.

### Volets côte à côte
- **Autant de volets que vous voulez**, à droite, à gauche, en haut ou en bas, et imbriqués : **Ctrl+Maj+flèche** ou le bouton ⊞ de chaque volet.
- **Glisser un onglet sur le bord d'un volet** le place dans un nouveau volet de ce côté (un repère bleu montre où).
- Séparateurs déplaçables entre les volets. **F6** passe d'un volet à deux volets côte à côte (et inversement), **Tab** passe au volet suivant, **Ctrl+Maj+F4** ferme le volet.
- **Ctrl+1 / Ctrl+2** : copier / déplacer la sélection vers l'autre volet (le dernier utilisé qui affiche un autre dossier).
- Le volet actif a une barre bleue ; le panneau latéral, l'aperçu, la barre d'état et les menus le suivent. Dans un volet étroit, la barre d'adresse se compacte.
- Volets, onglets et proportions sont retrouvés au prochain lancement.

### Glisser-déposer
- **Glisser des fichiers depuis Navis** vers l'Explorateur, le Bureau ou n'importe quel logiciel (navigateur, messagerie, éditeur…).
- **Déposer dans Navis** des fichiers venant de l'Explorateur ou d'un autre logiciel : dans la liste, sur un dossier de la liste, dans la vue en colonnes, sur un lecteur ou un dossier du panneau latéral, ou sur le panneau d'aperçu (dossier affiché).
- Mêmes règles que Windows : déplacer sur le même disque, copier vers un autre ; **Ctrl** = copier, **Maj** = déplacer, **Alt** = créer un raccourci. Glisser avec le **clic droit** : menu Copier / Déplacer / Créer des raccourcis.
- Le dossier visé est mis en évidence ; survoler un dossier 0,7 s le déplie pour viser un sous-dossier.

### Téléchargements
- Le dossier **Téléchargements** s'ouvre trié du plus récent au plus ancien, dossiers mêlés aux fichiers, avec un filtre **7 derniers jours** : vos derniers téléchargements sont tout en haut.
- Barre de filtre **Aujourd'hui / 7 jours / 30 jours / Tout**, avec le nombre d'éléments plus anciens masqués. Le choix et le tri sont mémorisés pour ce dossier.
- Le même filtre est disponible dans n'importe quel dossier : **Affichage > Filtrer par date de modification**.

### Corrections
- Au démarrage, et après un dépôt venu d'un autre logiciel, le clavier est directement dans la liste.
- Après un collage, la copie créée (« Nom - Copie ») est sélectionnée, et non plus l'original.
- Taper un nom qui contient des espaces sélectionne bien le fichier (l'espace n'ouvre plus l'aperçu rapide au milieu de la saisie).

## 0.4.0 — 4 novembre 2026

### Mises à jour automatiques
- Au démarrage (au plus une fois par jour), Navis vérifie s'il existe une nouvelle version sur GitHub.
- Si oui, un bandeau propose **Installer et redémarrer** : le téléchargement et le remplacement de l'exe se font tout seuls, puis Navis rouvre le dossier où vous étiez.
- Menu **Aide** : « Rechercher les mises à jour », vérification automatique activable ou non, « À propos de Navis ».
- Sécurité : le fichier téléchargé est vérifié avant de remplacer l'exe ; en cas de problème, l'ancienne version reste en place.

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
