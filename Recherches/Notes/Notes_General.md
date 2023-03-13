# Notes Générales

## Le MMR

### Table des matières

1) [Table des matières](#table-des-matières)
1) [Sources](#sources)
1) [Introduction](#introduction)
1) [Qu'est-ce qu'un MMR ?](#quest-ce-quun-mmr)
1) [Pourquoi créer un système de MMR ?](#pourquoi-créer-un-système-de-mmr)
1) [Calcul du MMR](#calcul-du-mmr)
1) [Attribution d'un MMR à un niveau](#attribution-dun-mmr-à-un-niveau)
1) [Visibilité du MMR](#visibilité-du-mmr)
1) [Valeurs extrêmes du MMR](#valeurs-extrêmes-du-mmr)
1) [Courbe d'évolution du MMR](#courbe-dévolution-du-mmr)
1) [Décroissance passive du MMR pour inactivité ?](#décroissance-passive-du-mmr-pour-inactivité)
1) [Notes de bas de page](#notes-de-bas-de-page)

### Sources

- [What does MMR mean in gaming?](https://dotesports.com/general/news/what-does-mmr-mean-in-gaming)
- [What does "MMR" mean in gaming? Explained](https://hitmarker.net/what-does-mmr-mean)

### Introduction

L'objectif du projet est de confronter l'élève à des exercices de difficulté différentes sur un même sujet, selon leur niveau de connaissance et les éléments du sujet à travailler.

Il faut donc trouver un moyen de faire correspondre le niveau de difficulté idéal auxquel le joueur doit être confronté.

C'est le rôle du MMR.

### Qu'est-ce qu'un MMR ?

Un MMR (abréviation de *Matchmaking Rating*) est un algorithme utilisé pour déterminer le niveau d'un joueur, principalement dans les jeux compétitifs avec classement.

### Pourquoi créer un système de MMR ?

> Quels seraient les objectifs qui pourraient être atteints grâce à un système de MMR ?

Les objectifs de l'instauration d'un système de MMR dans le projet seraient multiples :

- Mesurer l'évolution des connaissances et aptitudes du joueur.
- Placer le joueur face à des exercices lui permettant de solidifier ses connaissances acquises.
- Placer le joueur face à des exercices lui permettant d'acquérir de nouvelles connaissances. Ces connaissances peuvent être des sujets entièrement nouveaux ou des subtilités qui ne sont pas acquises d'un sujet déjà traité.
- Évaluer quelles sont les points de matière avec lesquels l'élève a plus de facilités ou de difficultés afin d'y remédier dans un second temps.

### Calcul du MMR

> **Comment calculer le MMR** ? Doit-il représenter une valeur unique ou doit-il être décomposé ? Selon quels critères ?

### Attribution d'un MMR à un niveau

> À qui sera attribuée la mission de définir la position d'un niveau dans la courbe de difficulté ? Comment sera réalisée cette mission ?

### Visibilité du MMR

> Le MMR d'un joueur sur un niveau doit-il être visible ? Qu'en est-il du MMR nécessaire pour débloquer un niveau ?

### Valeurs extrêmes du MMR

> Qu'en est-il des **valeurs plancher et plafond** qui doivent être attribuées au MMR d'un niveau/exercice ? Doit-il y en avoir ? Si oui, comment les définir, et pourquoi ? Si non, jusqu'où peuvent grimper ou diminuer les valeurs de MMR ? 

Pour ce qui est de la valeur plafond, il peut être intéressant d'en fixer une. En effet, selon la complexité d'un niveau/exercice, il peut être plus ou moins simple d'en atteindre une compréhension parfaite du sujet traité. Il est donc statistiquement plus que possible que certains élèves arrivent à réaliser des suites de réussite d'un même niveau arrivant à des valeurs monstrueusement élevées.<sup>2</sup>

Pour la valeur plancher, la question est plus complexe. En effet, il existera deux catégories majeures de niveaux/exercices qui influenceront la réponse : les niveaux d'introduction à un sujet, autrement dit les niveaux ne comprenant pas de niveau en prérequis, et les niveaux comprenant des niveaux en prérequis.  
Les niveaux faisant partie de la première catégorie sont plus simples à traiter car, ne nécessitant pas de prérequis, un échec représenterait obligatoirement un échec à la matière vue lors du niveau. En revanche, pour les niveaux comprenant des prérequis, un échec peut aussi être causé par une incompréhension d'un prérequis ou d'un détail de celui-ci, qui amène à une mauvaise compréhension de la matière vue lors du niveau.  
Pour la première catégorie, une valeur plancher peut être imaginée. Mais pour la deuxième catégorie de niveau, il faut être capable de distinguer les différentes causes possibles. Si une valeur plancher est envisagée, il faut tout de même être capable de répercutée d'une manière ou d'une autre les causes diagnostiquées d'un échec, soit-elles l'échec à la matière en elle-même ou l'échec à un (ou plusieurs) prérequis.

### Courbe d'évolution du MMR

> Qu'en est-il de la **courbe d'évolution** (à la hausse comme à la baisse) d'un MMR de niveau/exercice ? Quelle sera sa forme ? Sera-t-elle considérée comme simple ou les facteurs entrant en compte la rendront plus complexe ?

La réponse à ces questions peut aussi aider à répondre aux questions concernant les valeurs plancher/plafond d'un MMR.

Les parties de la courbe d'évolution d'un niveau les plus faciles à imaginer sont les deux extrêmes : la réussite extrême (de très nombreuses validations du niveau d'affilée) et l'échec extrême (de très nombreux échecs d'un niveau d'affilée). En effet, une courbe d'évolution linéaire du MMR pour ces parties-là ne seraient pas crédible. Il n'est pas possible d'évoluer encore plus que la perfection, et plus on s'en rapproche, au plus l'évolution est compliquée. Idem pour l'extrême opposé : si on ne comprend/connais absolument rien de la matière nécessaire à la réussite du niveau, il est impossible de connaître/comprendre encore moins la matière. La valeur de diminution du MMR à cet extrême doit aussi être minime.

Cette explication a deux objectifs : Si un MMR baisse trop vite dans la défaite, il sera d'autant plus long et répétitif d'essayer pour le joueur d'obtenir un meilleur MMR s'il vient à comprendre la matière. Cette longueur peut rapidement devenir frustration et démotivation. Il est important d'éviter la démotivation car elle peut amener à un abandon. L'abandon signifie un arrêt de la progression, alors que lui donner l'impression de progresser aura l'effet inverse : s'il pense qu'il progresse, le joueur aura envie de continuer à s'améliorer, ce qui renforcera aussi sa confiance en lui et son attitude sérieuse vis-à-vis de la matière travaillée.

Deuxième objectif : Un joueur proche de la perfection n'est pas totalement parfait. La maîtrise ultime est possible, mais la maîtrise parfaite ne l'est pas. Aussi, le joueur peut venir à oublier certains détails au fil du temps. Lorsqu'il revient sur un niveau pour lequel il a atteint le niveau de connaissance ultime, mais qu'il a oublié certains détails, il risque d'être démotivé par le niveau extrêmement élevé de l'exercice qui lui est proposé. De nombreux échecs à la suite en seront une conséquence possible, ce qui fera litérallement dégringoler son MMR.

Ce deuxième objectif est aussi un point de départ pour la question relative à une diminution passive du MMR pour inactivité.

### Décroissance passive du MMR pour inactivité ?

> Un système de décroissance du MMR pour inactivité doit-il être instauré pour les niveaux dont la matière n'a pas été retravaillée depuis un certain temps ? Sous quelle forme ?

### Notes de bas de page

<sup>1</sup> : Dans cette note, on parle d'un système de MMR, accronyme du terme *Matchmaking Rating*. Ce terme est principalement utilisé pour des jeux vidéo joueur-contre-joueur. Ici, puisqu'il est question d'un jeu vidéo orienté joueur-contre-niveau (ou joueur-contre-ordinateur), le niveau de difficulté ne servira pas à placer le joueur contre d'autres joueurs d'un niveau approximativement semblable au sien, mais plutôt face à des exercices dont la difficulté est appropriée à son niveau de connaissance afin qu'il puisse apprendre différents éléments par la pratique.  
Il est donc nécessaire d'adapter le terme MMR pour le faire mieux correspondre à ce que l'on cherche. *Level Matchmaking Rating* (noté LMMR) peut être un de ces termes plus adapté.  
Néanmoins, par facilité, cette note sera écrite avec le terme MMR.

<sup>2</sup> : Une idée supplémentaire est la création d'exercices "secrets", exercices auxquels seuls les joueurs ayant atteints un certain niveau de connaissance dans un niveau - ou une combinaison de niveaux - pourraient accéder.
