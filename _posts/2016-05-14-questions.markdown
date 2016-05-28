---
title: questions
layout: post
---
Comment faire les choses de manière répétitive de façon plus efficace?

Je remarque que je fais certaines choses de façon répétée.

Exemple: en ligne de commande, je cherche à faire un copié collé, de
dossiers dans un sous dossier -un déplacement- de tout ce qui est ici
dans un nouveau sous-dossier. Avec une souris cela corresiponsd à :
- click droit dans le réperotir, nouveau dossie , donner le nom
   - ctrl-A, ctrl-click sur le nouveau dossier
     - déplacer le contenu à la souris

j'ai plusieures fois cherché à faire ces opérations et fini par faire
graphiquement l'opération. Je cherche à me déplacer rapidement dans une
console, au clavier car je veux automatiser ces actions.

Les opérations simples, je les connais, puisque je ne les cherche plus.
Comme pour toute chose, je ne saurais dire combien de temps j'ai pris
pour apprendre insert.

Problème du jour

Je m 'arrête dans mon etntrerpise de rassembler mes repertoires git dans
un seul et de créer un hook pour générer les pdf à chaque commit pour
apprendre à déplacer tout le contenu d'un nouveau sous-répertoire, en
ligne de commande, rapidement.

Pour un seul fichier, 2 commandes:

    mkdir -p nouveaux/dossiers; mv fichier $\_

Pour tous les fichiers, 2 commandes:
Ajouter dans ~/.bash\_profile (.bashrc)  la ligne pour activer extglob,
pour finalement ne pas le mettre là, faire `shopt -s extglob` pour
activer cette option qui va me permettre de faire en 2 commandes:

    mkdir -p nouveau; mv !(nouveau) nouveau

Ce qui déplace tout sauf nouveau dans nouveau

Pour déplacer tout y compris les dossiers .cachés, on active
temporarirement l'option dotglob

    shopt -s extglob dotglob
    mv !(nouveau) nouveau
    shopt -u dotglob


