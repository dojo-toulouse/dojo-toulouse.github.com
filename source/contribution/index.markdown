---
layout: page
title: "Comment contribuer ?"
comments: true
sharing: true
author: Nicolas Deverge
footer: true
---

Toutes les personnes qui souhaitent contribuer à des animations de coding dojos ou autres activités dans le cadre de l'artisanat logiciel sur Toulouse sont fortement invitées à le faire ! Toutes les initiatives sont acceptées :-)

Si vous ne savez pas comment vous y prendre, vous pouvez demander un coup de main à [Nicolas](http://twitter.com/ndeverge) ou [Antoine](http://twitter.com/avernois).

Si en plus, vous souhaitez communiquer pour votre évènements via ce blog, n'hésitez surtout pas !

Pour cela, il suffit de savoir utiliser [Octopress](http://octopress.org/), c'est à dire :

* être un geek
* savoir utiliser Git
* avoir un environnement Rails (moi même je ne connais rien à Rails)
* avoir un compte github
* et c'est tout !

Pour ajouter un article, il suffit de forker le repository [dojo-toulouse.github.com](https://github.com/dojo-toulouse/dojo-toulouse.github.com) et de le cloner sur son poste.

Pour créer un article :

```
rake new_post["title"]
```

L'article est créé dans `source/_posts/YYYY-MM-DD-title.markdown`. Ensuite, il faut l'écrire avec la syntaxe markdown.

Pour prévisualiser son article en local sur son ordi :

```
rake generate
rake preview
```

Plus de détails sur le site d'Octopress : [Blogging Basics](http://octopress.org/docs/blogging/)

Ensuite, il suffit de pusher vos modifications sur Github, vous faites une pull request et on publie l'article !
