# Introduction à la programmation en C++

Recueil de travaux pratiques de première année (cursus ТКИ), écrits en C++ et
documentés au format Doxygen (commentaires en russe). Chaque tâche isole une
notion : fonctions et formules, saisie clavier, branchements, boucles et
tableaux.

## Organisation

Le dépôt est structuré en quatre séries de trois exercices, chacun dans son
propre sous-dossier avec son `main.cpp` :

| Série | Thème | Exercices |
|---|---|---|
| **Task 1** | Fonctions et évaluation de formules | calcul multi-variables `f(x,y,z)` · conversion de poids · travail d'un moteur électrique (I, U) |
| **Task 2** | Fonctions à plusieurs sorties | périmètre & aire d'un rectangle · fonction définie par morceaux · temps de trajet cumulé |
| **Task 3** | Branchements et séries | domaine de définition d'une fonction · somme d'une suite récurrente · évaluation ponctuelle |
| **Task 4** | Tableaux | trois traitements de tableaux saisis à l'exécution |

Chaque exercice suit la même convention : prototypes documentés en tête de
fichier, `main()` pour les entrées/sorties, puis définition des fonctions.

## Compilation et exécution

Chaque exercice est autonome. Depuis la racine du dépôt :

```bash
g++ -std=c++17 "Task 1/Task 1 - 1/main.cpp" -o task1-1
./task1-1
```

Les programmes lisent leurs paramètres sur l'entrée standard. Les intitulés et
messages affichés sont en russe.

## État de compilation

Les treize exercices compilent sans erreur avec `g++ -std=c++17`, vérifié par
compilation de chacun. Deux corrections ont été nécessaires (voir l'historique
git) : une constante non initialisée lue au clavier dans `Task 1 - 2`, et dans
`Task 3-2` un compte mal récupéré, une somme qui retournait toujours `0.0` et un
argument par défaut dupliqué.
