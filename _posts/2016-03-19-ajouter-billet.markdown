---
layout: post
title:  Nouveau billet
date:   2016-03-19 19:30:10 -0400
---
Les billets sont dans le répertoire `_post`.

Ils doivent commencer par le code suivant, pour le fuseau horaire de Montréal.

{% highlight markdown %}
---
layout: post
title:  "titre billet"
date:    yyyy-mm-jj hh:mm:ss -0400
categories: jekyll, teaching, new
---
{% endhighlight %}

Le caractère (accent grave) utilisé en paire échappe le contenu `de cette façon`.

Pour faire un lien, écrire le texte de lien entre crochets suivi de la référence aussi entre crochets [Mon lien][ref-abc] : `[Mon lien][ref-abc]`.

En bas de la page, on met le lien de la référence:

`[ref-abc]: http://google.com`

[ref-abc]: http://google.com
