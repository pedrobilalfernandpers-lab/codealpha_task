🚀 Stage en Ligne chez CodeAlpha — Programmation C
Stagiaire : PEDRO Bilal
Projet : Tâche 2 — Conception d'un Module d'Algèbre Matricielle en C
📝 Description du projet
Dans le cadre de ma deuxième tâche de stage chez CodeAlpha, j'ai développé un Calculateur de Matrices classique s'exécutant entièrement en mode console. L'objectif est de permettre à l'utilisateur de manipuler des matrices bidimensionnelles à travers des opérations fondamentales d'algèbre linéaire. Conformément aux bonnes pratiques de modularité en C, ce programme s'appuie sur une allocation statique définie par une dimension maximale (⁠MAX = 10⁠) et implémente des fonctions dédiées pour la saisie, l'affichage et les calculs algorithmiques afin d'éviter la redondance de code.
⚙️ Logique Fonctionnelle & Règles Implémentées
Le script intègre une gestion rigoureuse des structures de données bidimensionnelles à chaque étape de l'exécution :
 Saisie Sécurisée et Guidée : Le programme invite l'utilisateur à remplir chaque case de la matrice de manière itérative en affichant explicitement les indexations courantes sous un format humainement lisible (ex: ⁠Element [1][1]⁠, ⁠Element [1][2]⁠).
 Affichage Tabulaire Clair : Les résultats des opérations sont formatés sous forme de grille grâce à l'utilisation d'espacements tabulaires (⁠\t⁠), assurant un alignement parfait des lignes et des colonnes dans le terminal.
 Calcul d'Addition : Effectue une somme terme à terme de deux matrices de dimensions identiques, garantissant un résultat linéaire direct.
 Calcul de la Multiplication : Implémente le produit matriciel classique (ligne par colonne) à l'aide d'une triple boucle imbriquée, combinant des opérations de multiplication et d'accumulation cumulative.
 Calcul de la Transposée : Permute dynamiquement les lignes et les colonnes d'une matrice cible (les éléments ⁠m[i][j]⁠ deviennent ⁠res[j][i]⁠), permettant de basculer l'orientation spatiale de la structure.
🛠️ Concepts Clés Utilisés & Respectés
Pour structurer ce code de manière efficace et optimisée, les concepts fondamentaux suivants ont été mobilisés :
1. Directives de Préprocesseur (⁠#define⁠) : Utilisation d'une constante globale ⁠MAX⁠ fixée à 10 pour définir de manière sécurisée la taille maximale des tableaux statiques en mémoire.
2. Pointeurs et Tableaux Bidimensionnels : Passage de matrices en paramètres de fonctions (par adresse implicitée), permettant la modification directe des données sans duplication mémoire coûteuse.
3. Boucles ⁠for⁠ Imbriquées : Utilisation systématique de deux niveaux de boucles (compteurs ⁠i⁠ et ⁠j⁠) pour parcourir de façon exhaustive les lignes et les colonnes des structures de données.
4. Modularité par Fonctions : Découpage du code en blocs réutilisables distincts pour séparer la logique d'affichage (⁠afficher⁠), de saisie (⁠lire⁠) et de calcul (⁠addition⁠, ⁠multiplication⁠, ⁠transposee⁠).
🎮 Comment exécuter le programme
Assurez-vous de disposer d'un compilateur C (comme ⁠gcc⁠) installé sur votre environnement local, puis lancez les commandes suivantes depuis votre terminal :
gcc matrix_calc.c -o matrix_calc
./matrix_calc