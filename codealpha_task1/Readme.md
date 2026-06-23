# 🚀 Stage en Ligne chez CodeAlpha — Programmation C

**Stagiaire :** PEDRO Bilal FernanD-Pers
**Projet :** Tâche 1 — Conception d'un Programme Calculatrice Élémentaire

---

## 📝 Description du projet

Dans le cadre de ma première tâche de stage chez **CodeAlpha**, j'ai développé une **Calculatrice Algorithmique** classique s'exécutant entièrement en mode console. L'objectif est de permettre à l'utilisateur d'effectuer de manière fluide les quatre opérations arithmétiques fondamentales (Addition, Soustraction, Multiplication et Division) à partir de deux opérandes saisis dynamiquement. 

Conformément aux directives rigoureuses de conception logicielle et aux critères d'optimisation du stage, ce programme a été conçu pour structurer une logique séquentielle propre, robuste et parfaitement sécurisée contre les exceptions mathématiques critiques en programmation système.

---

## ⚙️ Logique Fonctionnelle & Règles Implémentées

Le script intègre une gestion rigoureuse du flux d'exécution et de l'analyse des données d'entrée :

* **Sélection de l'Opération :** L'architecture repose sur l'évaluation efficace d'une structure conditionnelle à choix multiples `switch-case` pour aiguiller instantanément le traitement vers l'opérateur arithmétique sélectionné (`+`, `-`, `*`, `/`).
* **Sécurisation Mathématique (Division par Zéro) :** Le programme vérifie de manière préventive le second opérande avant toute tentative de division. Si l'utilisateur saisit `0`, le système bloque immédiatement l'évaluation, intercepte l'erreur critique et affiche un message d'avertissement explicite pour empêcher le plantage du terminal (Crash de type *Floating Point Exception*).
* **Validation des Opérateurs :** Toute saisie d'un symbole non reconnu ou d'un opérateur invalide est traitée par la clause `default` du bloc, renvoyant une notification d'erreur dédiée sans exécuter de calcul erroné.
* **Précision des Calculs :** Utilisation de types de données adaptés (`float` / `double`) pour supporter les valeurs décimales, garantissant une précision optimale lors des opérations de division.

---

## 🛠️ Concepts Clés Utilisés & Respectés

Pour structurer ce code de manière performante et modulaire, les concepts fondamentaux suivants du langage C ont été mobilisés :

1.  **Instructions de Sélection Complètes (`switch...case`) :** Implémentation exclusive pour le branchement conditionnel de l'opération, évitant ainsi l'imbrication excessive de blocs `if-else` et optimisant la table des sauts à la compilation.
2.  **Opérateurs Arithmétiques Natifs :** Utilisation optimisée des symboles standards du langage pour le traitement direct au niveau du processeur.
3.  **Contrôle des Flux d'Entrée/Sortie (`stdio.h`) :** Gestion fine des fonctions de lecture `scanf()` et d'affichage formaté `printf()` avec formatage approprié des types de données.
4.  **Robustesse Algorithmique :** Intégration de filtres conditionnels de sécurité imbriqués pour la validation stricte des règles arithmétiques de base.

---

## 🎮 Comment exécuter le programme

Assurez-vous de disposer d'un compilateur C (comme `gcc`) installé sur votre environnement local (Ubuntu/Linux), puis lancez les commandes suivantes depuis votre terminal :

**Compilation du fichier source :**
```bash
gcc calculatrice.c -o calculatrice