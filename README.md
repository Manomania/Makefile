# Advanced C++ Makefile

Un Makefile moderne et feature-rich pour projets C++98 avec interface visuelle améliorée.

## ✨ Fonctionnalités

### 🎨 Interface visuelle
- **ASCII Art** : Logo CPP stylisé au démarrage
- **Couleurs** : Sortie colorée pour une meilleure lisibilité
- **Barre de progression** : Animation en temps réel pendant la compilation
- **Frames animées** : Spinner avec caractères Unicode

### 🔧 Compilation intelligente
- **Détection auto** : Détecte les fichiers modifiés uniquement
- **Dépendances** : Génération automatique des dépendances (`.d`)
- **Compilation incrémentale** : Recompile seulement le nécessaire
- **Support multi-core** : Détection automatique du nombre de CPU

### 📊 Informations système
- **Détection OS** : Linux, macOS, autres systèmes
- **Info compilateur** : Version et détails du compilateur
- **Statistiques** : Nombre de fichiers source/header
- **Progression** : Pourcentage de compilation en temps réel

## 🚀 Commandes

| Commande | Description |
|----------|-------------|
| `make` | Compilation standard avec interface visuelle |
| `make clean` | Supprime les fichiers objets |
| `make fclean` | Suppression complète |
| `make re` | Recompilation complète |
| `make help` | Affiche l'aide détaillée |
| `make info` | Informations système complètes |

## ⚙️ Configuration

### Variables principales
```makefile
AUTHOR    := maximart
NAME      := ex01
CC        := c++
CFLAGS    := -Wall -Wextra -Werror -std=c++98
```

### Structure de projet
```
project/
├── src/          # Sources (.cpp)
├── include/      # Headers (.hpp)
├── obj/          # Objets (auto-généré)
└── Makefile
```

## 🎯 Fonctionnalités avancées

### Barre de progression animée
- Animation avec frames Unicode (`⠋ ⠙ ⠹ ⠸ ⠼ ⠴ ⠦ ⠧ ⠇ ⠏`)
- Pourcentage en temps réel
- Indication visuelle de fin de compilation

### Détection intelligente
- **Compilation incrémentale** : Détecte les fichiers modifiés
- **Multi-platform** : Linux, macOS, systèmes compatibles
- **CPU cores** : Utilise `nproc` ou `sysctl` selon l'OS

### Interface colorée
- **Headers** : Informations projet en couleur
- **Progression** : Codes couleur pour le statut
- **Erreurs/succès** : Distinction visuelle claire

## 📋 Exemple de sortie

```
                            __________  ____
                           / ____/ __ \/ __ \
                          / /   / /_/ / /_/ /
                         / /___/ ____/ ____/
                         \____/_/   /_/

----------------------------------------------------------------------

AUTHOR:                                  maximart
NAME:                                    ex01
CC:                                      c++
FLAGS:                                   -Wall -Wextra -Werror -std=c++98

----------------------------------------------------------------------

[ex01]:
⠋ Compiling... [2/2] 100%
Compilation finished [2/2]                [✓]
```

## 🛠️ Personnalisation

Facilement adaptable :
- Modifier les variables en début de fichier
- Ajouter des fichiers dans `SRC_F` et `HDR_F`
- Personnaliser les couleurs et animations
- Adapter les flags de compilation

## 📦 Dépendances

- `bc` : Calculs de pourcentage
- `find` : Recherche de fichiers
- Modification manuelle du titre en ASCII ART (À automatiser dans une future update)
- Terminal compatible Unicode pour les animations

---

*Un Makefile qui rend la compilation... presque fun !*
