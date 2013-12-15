---
layout: page
title: "Comment contribuer ?"
comments: true
sharing: true
author: Nicolas Deverge
footer: true
---

Toutes les personnes qui souhaitent contribuer à des animations de coding dojos ou autres activités dans le cadre de l'artisanat logiciel sur Toulouse sont fortement invitées à le faire ! Toutes les initiatives sont acceptées :-)

Pour découvrir et s'enregistrer à un évènement, rendez-vous sur [meetup](http://www.meetup.com/Software-Craftsmanship-Toulouse/).

Si vous ne savez pas comment vous y prendre, vous pouvez demander un coup de main à [Nicolas](http://twitter.com/ndeverge) ou [Antoine](http://twitter.com/avernois).

Si en plus, vous souhaitez communiquer pour votre évènements via ce blog, n'hésitez surtout pas !

Pour cela, il suffit de savoir utiliser [Octopress](http://octopress.org/), c'est à dire :

* être un geek
* savoir utiliser Git
* avoir un environnement Rails (moi même je ne connais rien à Rails)
* avoir un compte github
* et c'est tout !

Première installation
---

Toute la doc est disponible sur le site octopress.

1. Installer ruby version 1.9.3 minimum
2. Forker le repo [dojo-toulouse.github.com](https://github.com/dojo-toulouse/dojo-toulouse.github.com) puis cloner la branche `source`.

```
git clone git@github.com:<username>/dojo-toulouse.github.com.git -b source
```

Blogguer
---
Pour créer un article :

```
rake new_post["title"]
```

L'article est créé dans `source/_posts/YYYY-MM-DD-title.markdown`. Ensuite, il faut l'écrire avec la syntaxe markdown.

Pour prévisualiser le blog en local :
```
rake preview
```

Puis rendez-vous sur `http://localhost:4000`.

Tous les détails pour ajouter des éléments (images, citations, code) sont sur le site d'Octopress : [Blogging Basics](http://octopress.org/docs/blogging/). N'hésitez pas à ajouter du code dans vos posts : [Sharing Code Snippets](http://octopress.org/docs/blogging/code/).

Déployer
---

Pour déployer vos modifications sur votre github :

```
rake generate
rake deploy
git push origin source
```

**Notez bien** qu'il n'est pas nécessaire de pusher `master` car c'est `rake generate` qui va s'en charger.

Ensuite, il suffit de faire une pull request et on publie l'article !
