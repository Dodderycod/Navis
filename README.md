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

## Ce que fait Navis

| | |
|---|---|
| **Vue Détails** | Rapide même sur des dossiers de milliers de fichiers, tri naturel, taille des dossiers calculée en arrière-plan |
| **Dossiers dépliables** | Flèche ▸ devant chaque dossier pour voir son contenu sans y entrer (Alt+clic : tous les sous-niveaux) |
| **Vue en colonnes** | Comme le Finder de macOS : chaque dossier sélectionné s'ouvre dans une colonne à droite |
| **Aperçus** | Images, texte, PDF, Word / Excel / PowerPoint, modèles 3D (STL, OBJ) dans le panneau d'aperçu (F7) |
| **Aperçu rapide** | Barre Espace, avec une animation de zoom |
| **Recherche** | `*.exe`, `*.(png\|jpg)`, `taille:>100mo`, `date:<7j`, `regex:`… dans le dossier courant et ses sous-dossiers |
| **Index** | Résultats en moins d'un quart de seconde sur tout un disque, mis à jour en direct |
| **Lecteurs** | Tous les disques, clés USB et lecteurs réseau dans le panneau latéral, avec leur espace libre |
| **Menu Windows** | Le vrai menu clic droit (7-Zip, Git, Envoyer vers…), en plus des actions de Navis |

## Raccourcis utiles

| Raccourci | Action |
|---|---|
| Espace | Aperçu rapide |
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
