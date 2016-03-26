---
layout: post
title:  "À propos de la simplicité d'utilisation de jekyll"
date:   2016-03-23 20:37:14
categories: jekyll
---

## Retour d'expérience

Jekyll permet de faire des pages web très rapidement, grâce à git/hub. 
Il suffit de se souvenir de quelques commandes pour faire les opérations nécessaires.

Git et github permettent de mettre en place un workflow, un enchainement d'étapes qui rendent le travail confortable.

Travailler avec git par terminal et vim demande d'être bon en orthographe. Mais les alternatives graphiques sont performantes.

## Aide mémoire

* ### Cloner/rafraîchir le dépot

Toutes les sources sont automatiquement téléchargées dans l'emplacement de travail. Cela peut se faire avec le GUI de git, vers le dépot de [github][github].


* ### Travailler dans la branche de développement

À chacun ses méthodes, ce qui compte c'est de faire des changements au site selon les possibilités offertes par Jekyll.

* ### Démarrer le serveur local, à partir du dossier de travail

`jekyll serve`

* ### Ouvrir dans le navigateur, la copie de travail

Par défaut, le serveur local se trouve en : [localhost:4000][lien-local]

* ### Quand la copie de développement est prête à être mis en ligne

```bash
  git checkout master
  git merge branchedev
```
  Ou toute autre technique GUI pour mettre sur origin/master la copie de développement.

---

Ensuite, on peut [ajouter un nouveau billet]({% post_url 2016-03-19-ajouter-billet %})

[github]: https://github.com/sgdjs/sgdjs.github.io.git
[lien-local]: http://localhost:4000
