<p align="center">
  <img src="logo.png" width="128" alt="Logo de Navis" />
</p>

<h1 align="center">Navis</h1>

<p align="center">
  Un explorateur de fichiers rapide et sombre pour Windows 10 et 11.<br/>
  Dossiers dépliables, vue en colonnes, aperçus instantanés et recherche ultra-rapide.
</p>

<p align="center">
  <a href="../../releases/latest"><b>⬇ Télécharger la dernière version (Navis.exe)</b></a>
</p>

---

## Installation

1. Téléchargez **`Navis.exe`** depuis la [dernière release](../../releases/latest).
2. Lancez-le : il n'y a rien à installer. L'exe est autonome et n'a pas besoin de .NET.
3. Au premier lancement, Windows peut afficher « Windows a protégé votre ordinateur » : l'application n'est pas
   signée numériquement. Cliquez sur **Informations complémentaires**, puis sur **Exécuter quand même**.

Configuration : Windows 10 ou 11, 64 bits. Les réglages sont enregistrés dans `%AppData%\Navis`.

**Mises à jour** : à partir de la version 0.4.0, Navis vérifie lui-même s'il existe une nouvelle version
(au plus une fois par jour) et propose de l'installer d'un clic. Vous pouvez aussi passer par le menu
**Aide > Rechercher les mises à jour**. Si vous avez la version 0.3.0, téléchargez une dernière fois
la nouvelle version à la main.

## Ce que fait Navis

| | |
|---|---|
| **Onglets et volets** | Plusieurs onglets, et autant de volets que vous voulez côte à côte, empilés ou imbriqués ; glisser un onglet sur un bord pour créer un volet |
| **Vue Détails** | Rapide même sur des dossiers de milliers de fichiers, tri naturel, taille des dossiers calculée en arrière-plan |
| **Dossiers dépliables** | Flèche ▸ devant chaque dossier pour voir son contenu sans y entrer (Alt+clic : tous les sous-niveaux) |
| **Vue en colonnes** | Comme le Finder de macOS : chaque dossier sélectionné s'ouvre dans une colonne à droite |
| **Aperçus** | Images, texte, PDF, Word / Excel / PowerPoint, modèles 3D (STL, OBJ) dans le panneau d'aperçu (F7) |
| **Aperçu rapide** | Barre Espace, avec une animation de zoom |
| **Recherche** | `*.exe`, `*.(png\|jpg)`, `taille:>100mo`, `date:<7j`, `regex:`… dans le dossier courant et ses sous-dossiers |
| **Index** | Résultats en moins d'un quart de seconde sur tout un disque, mis à jour en direct |
| **Lecteurs** | Tous les disques, clés USB et lecteurs réseau dans le panneau latéral, avec leur espace libre |
| **Menu Windows** | Le vrai menu clic droit (7-Zip, Git, Envoyer vers…), en plus des actions de Navis |
| **Glisser-déposer** | Avec l'Explorateur et tous les logiciels, dans les deux sens ; Ctrl / Maj / Alt et clic droit comme dans Windows |
| **Téléchargements** | Les plus récents en haut, filtre Aujourd'hui / 7 jours / 30 jours / Tout |
| **Mises à jour** | Vérification automatique et installation en un clic, sans quitter l'application |

## Raccourcis utiles

| Raccourci | Action |
|---|---|
| Espace | Aperçu rapide |
| Ctrl+T / Ctrl+W | Nouvel onglet / fermer l'onglet |
| Ctrl+Maj+T | Rouvrir le dernier onglet fermé |
| Ctrl+Tab | Onglet suivant |
| Ctrl+Maj+flèche | Diviser le volet (droite, gauche, haut, bas) |
| F6 / Tab | Deux volets côte à côte / volet suivant |
| Ctrl+1 / Ctrl+2 | Copier / déplacer vers l'autre volet |
| Ctrl+F | Rechercher dans le dossier |
| Droite / Gauche | Déplier / replier un dossier |
| Alt+Gauche / Alt+Droite | Précédent / Suivant |
| Retour arrière | Dossier parent |
| F2 | Renommer |
| Suppr / Maj+Suppr | Corbeille / suppression définitive |
| Ctrl+Maj+N | Nouveau dossier |
| Ctrl+Maj+L / Ctrl+Maj+D | Vue en colonnes / vue Détails |
| F7 / F8 | Panneau d'aperçu / panneau latéral |
| Ctrl+D | Épingler le dossier à l'accès rapide |

## Syntaxe de recherche

| Exemple | Effet |
|---|---|
| `*.exe` | tous les fichiers .exe |
| `*.exe *.dll` | l'un ou l'autre |
| `*.(png\|jpg)` | alternatives |
| `rapport 2024` | les deux mots, n'importe où dans le nom |
| `"mon fichier"` | texte avec espaces |
| `*.cs ~*.g.cs` | exclure |
| `regex:^img\d+` | expression régulière |
| `type:dossier`, `ext:png,jpg` | type ou extension |
| `taille:>100mo`, `date:<7j`, `date:>2026-01-01` | taille ou date de modification |

## Nouveautés

<!-- Le contenu ci-dessous est recopié automatiquement depuis CHANGELOG.md par Publier.bat. -->
### 0.5.0 — 12 novembre 2026

#### Onglets
- **Plusieurs onglets** par volet, chacun avec son dossier et son historique Précédent / Suivant.
- **Ctrl+T** nouvel onglet, **Ctrl+W** fermer, **Ctrl+Maj+T** rouvrir le dernier onglet fermé, **Ctrl+Tab** / **Ctrl+Maj+Tab** onglet suivant / précédent.
- **Clic du milieu** sur un dossier : il s'ouvre dans un nouvel onglet. Clic du milieu sur un onglet : il se ferme. Double-clic dans la barre d'onglets : nouvel onglet.
- Glisser un onglet pour le réordonner ou le mettre dans un autre volet. Clic droit : dupliquer, fermer les autres, fermer ceux de droite, déplacer dans un nouveau volet.
- En changeant d'onglet, la sélection et le défilement sont retrouvés.

#### Volets côte à côte
- **Autant de volets que vous voulez**, à droite, à gauche, en haut ou en bas, et imbriqués : **Ctrl+Maj+flèche** ou le bouton ⊞ de chaque volet.
- **Glisser un onglet sur le bord d'un volet** le place dans un nouveau volet de ce côté (un repère bleu montre où).
- Séparateurs déplaçables entre les volets. **F6** passe d'un volet à deux volets côte à côte (et inversement), **Tab** passe au volet suivant, **Ctrl+Maj+F4** ferme le volet.
- **Ctrl+1 / Ctrl+2** : copier / déplacer la sélection vers l'autre volet (le dernier utilisé qui affiche un autre dossier).
- Le volet actif a une barre bleue ; le panneau latéral, l'aperçu, la barre d'état et les menus le suivent. Dans un volet étroit, la barre d'adresse se compacte.
- Volets, onglets et proportions sont retrouvés au prochain lancement.

#### Glisser-déposer
- **Glisser des fichiers depuis Navis** vers l'Explorateur, le Bureau ou n'importe quel logiciel (navigateur, messagerie, éditeur…).
- **Déposer dans Navis** des fichiers venant de l'Explorateur ou d'un autre logiciel : dans la liste, sur un dossier de la liste, dans la vue en colonnes, sur un lecteur ou un dossier du panneau latéral, ou sur le panneau d'aperçu (dossier affiché).
- Mêmes règles que Windows : déplacer sur le même disque, copier vers un autre ; **Ctrl** = copier, **Maj** = déplacer, **Alt** = créer un raccourci. Glisser avec le **clic droit** : menu Copier / Déplacer / Créer des raccourcis.
- Le dossier visé est mis en évidence ; survoler un dossier 0,7 s le déplie pour viser un sous-dossier.

#### Téléchargements
- Le dossier **Téléchargements** s'ouvre trié du plus récent au plus ancien, dossiers mêlés aux fichiers, avec un filtre **7 derniers jours** : vos derniers téléchargements sont tout en haut.
- Barre de filtre **Aujourd'hui / 7 jours / 30 jours / Tout**, avec le nombre d'éléments plus anciens masqués. Le choix et le tri sont mémorisés pour ce dossier.
- Le même filtre est disponible dans n'importe quel dossier : **Affichage > Filtrer par date de modification**.

#### Corrections
- Au démarrage, et après un dépôt venu d'un autre logiciel, le clavier est directement dans la liste.
- Après un collage, la copie créée (« Nom - Copie ») est sélectionnée, et non plus l'original.
- Taper un nom qui contient des espaces sélectionne bien le fichier (l'espace n'ouvre plus l'aperçu rapide au milieu de la saisie).

### 0.4.0 — 4 novembre 2026

#### Mises à jour automatiques
- Au démarrage (au plus une fois par jour), Navis vérifie s'il existe une nouvelle version sur GitHub.
- Si oui, un bandeau propose **Installer et redémarrer** : le téléchargement et le remplacement de l'exe se font tout seuls, puis Navis rouvre le dossier où vous étiez.
- Menu **Aide** : « Rechercher les mises à jour », vérification automatique activable ou non, « À propos de Navis ».
- Sécurité : le fichier téléchargé est vérifié avant de remplacer l'exe ; en cas de problème, l'ancienne version reste en place.

### 0.3.0 — 4 novembre 2026

Première version publique.

#### Explorer
- Vue **Détails** rapide (dossiers de plus de 5 000 éléments affichés en moins d'une seconde), tri naturel (`fichier2` avant `fichier10`), dossiers en premier.
- **Dossiers dépliables sur place** : flèche ▸ / ▾, Alt+clic pour tout déplier (5 niveaux), Ctrl+Alt+Gauche pour tout replier ; l'état déplié est gardé dans l'historique.
- **Vue en colonnes** façon Finder (Ctrl+Maj+L).
- **Taille des dossiers** calculée en arrière-plan.
- **Panneau latéral** (F8) : accès rapide, dossiers épinglés (Ctrl+D), tous les lecteurs avec leur espace libre.

#### Aperçus
- **Panneau d'aperçu** (F7) : images, texte et code, PDF, Word / Excel / PowerPoint, modèles 3D STL et OBJ ; chaque type peut être désactivé.
- **Aperçu rapide** avec la barre Espace, animation de zoom façon macOS.

#### Fichiers
- Clic droit : actions de base, et le **vrai menu Windows** (7-Zip, Git, Envoyer vers…).
- Couper / copier / coller compatibles avec l'Explorateur, Corbeille, renommage sur place (F2), nouveau dossier (Ctrl+Maj+N).
- Mise à jour automatique quand un fichier change.

#### Recherche
- **Recherche** dans le dossier courant et ses sous-dossiers (Ctrl+F) : `*.exe`, `*.(png|jpg)`, mots, `~exclure`, `regex:`, `type:dossier`, `taille:>100mo`, `date:<7j`…
- **Index de recherche** : résultats en moins d'un quart de seconde sur tout un disque, mis à jour en direct (menu Outils > Index de recherche).
