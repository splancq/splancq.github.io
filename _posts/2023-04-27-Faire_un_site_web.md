---
title:  "Faire un site web avec GitHub Pages et Jekyll"
layout: post
categories: media
---

![jekyll and github](https://scriptedtea.com/assets/images/posts/jekyll_pages.jpg)



A l'heure actuelle il est étonnement facile d'avoir son propre site web. En effet, tant que l'on a uniquement besoin d'un [site statique](https://fr.wikipedia.org/wiki/Page_web_statique), on peut déléguer le gros du travail informatique à des logiciels tiers. Ainsi on peut in fine écrire nos pages en casi langage naturel. Le site web ici présent utilise [GitHub Pages](https://pages.github.com/), qui va s'occuper d'héberger le site. Le gros avantage de passer par github pages est qu'on a accès gratuitement à une adresse web basé sur notre compte GitHub : idéal pour commencer sans s'occuper de trouver un nom de domaine.

GitHub Pages utilise Jekyll pour générer le site web. C'est Jekyll qui va convertir des fichiers text [markdown](https://fr.wikipedia.org/wiki/Markdown) en pages web. Il a une [documentation](https://jekyllrb.com/docs/) très complète avec entre autre de [nombreux exemples](https://jekyllrb.com/showcase/) de site se basant sur Jekyll, et qui en montre la polyvalence.

# Faire son site web
Mais comment faire en pratique ? Je recommande chaudement la vidéo que j'ai utilisée, où Kathryn Schuler montre que l'on peut avoir un site web fonctionnel en 25mn~. Quelques petites remarques pour vous avant de voir la vidéo : déjà GitHub met quelques minutes à générer le site web, d'où parfois un délais entre la mise à jour sur GitHub et l'affichage sur le net. Aussi, depuis la sortie de la vidéo il faut aussi aller dans les paramètres du projet GitHub pour faire marcher GitHub Pages (`settings -> GitHub Pages -> sélectionner comme branch 'master'`). 
<!---
Enfin dans la vidéo Kathryn n'arrive pas à mettre son CV. Cela est probablemnt du (comme le dit )
https://github.com/MihajloNesic/jekyll-pdf-embed
-->

{% include embed.html url="https://www.youtube.com/watch?v=qZsgPgGdOzQ" %}

Si le thème Jekyll [contrast](https://github.com/niklasbuschmann/contrast) utilisé dans la vidéo ainsi que pour ce site ne vous convient pas, il existe de [nombreux thèmes](http://jekyllthemes.org/) disponible gratuitement et qui utilise la même logique (fork le projet et adapter à ses besoins).

Jekyll possède d'autre fonctionnalités que celles présentées dans la vidéo, comme par exemple une gestion de tags, mais je ne l'ai pas encore assez pris en mains pour pouvoir en parler.

# Les limites

Premièrement, à moins que vous n'ayez un compte github professionnel, votre code source GitHub Pages est publique. Cela signifie que n'importe qui aura accès au code source de votre site web (et pas seulement aux pages web générées par Jekyll). Autre point important : GitHub Pages est conçu pour des sites statiques, et n'a donc pas forcement les mesures de sécurité réseau que l'on souhaite avoir dès lors que l'on a un site dynamique (par exemple vis à vis de la sécurité des mots de passes). Aussi je vous conseille de partir du principe que tout ce que vous mettrez sur votre dossier GitHub sera librement visible sur internet : n'y mettez jamais d'informations que vous ne souhaitez pas etre connus de tous (comme un numéro de téléphone ou une adresse mail perso par exemple).

De plus la taille maximale du dossier git qui génère le site ne peux pas dépasser 1Go. Cela peut paraitre comme beaucoup mais est atteignable si l'on met beaucoup d'images directement dans le dossier. Aussi je conseillerai d'utiliser les liens web des images plutôt que de les mettre dans votre dossier, et au besoin de mettre vos images sur un site d'hébergement d'image comme [imgur](https://imgur.com/).