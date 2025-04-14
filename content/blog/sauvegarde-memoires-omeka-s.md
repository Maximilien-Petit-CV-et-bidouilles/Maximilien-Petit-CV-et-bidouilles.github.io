---
date: '2025-04-14T09:12:24+02:00'
draft: false
title: 'Mettre en place un circuit de sauvegarde des mémoires avec Omeka S'
author: Maximilien Petit
tags: ["Omeka S"]
readingTime: true
---
{{< toc >}}

# Le problème

**Les mémoires de Master ne font pas l'objet d'un circuit de dépôt légal comme c'est le cas pour les thèses**. Même s'il y a des projets en cours pour inventorier et localiser des mémoires sur certains sujets (par exemple, <a href="https://19m.nakalona.fr/" target="_blank">la base XIXe siècle en mémoires</a>), le fait étant que les piles de mémoires, dans les unités de recherche, prennent la poussière sur les étagères dans les laboratoires ou terminent dans une benne une fois par an. Au mieux, dans certaines universités, on conserve les PV de soutenance qui sont une trace administrative et certains enseignants-checheurs gardent une copie (numérique ou papier) et tiennent à jour des bibliographies des mémoires qu'ils suivent. **Il y a donc une gestion "au fil de l'eau" et tous les acteurs (administratifs et pédagogiques) font ce qu'ils peuvent**.

**Pourtant, selon moi, il y a un intérêt à mettre en place localement (à l'échelle d'une composante) un circuit de sauvegarde des mémoires. Et si circuit il y a, il doit être dématérialisé** car il n'y a plus vraiment de place physique dans les unités de recherche pour entretenir de grosses collections. Les mémoires n'ont certes pas toujours une qualité suffisante aux yeux des enseignants-chercheurs mais **ils sont le reflet à un instant T d'un travail bibliographique et d'une orientation pédagogique** donc il peut être intéressant de les conserver. En particulier pour les étudiants à venir qui, souvent, en M1, veulent ouvrir un mémoire, savoir ce que c'est concrètement, et comment cela se "construit". **Savoir ce qu'il faut faire, et ce qu'il ne faut pas faire**.

## Qui peut aider ? 

Les enseignants-chercheurs qui ont la charge de diriger les promotions de Master, et les personnels de la filière bibliothèque.

## La bidouille

Le résultat visible ici : <a href="https://bibliohisto.org/s/bibliohisto/page/masters" target="_blank">Les masters HCS 2023-2024 sur Bibliohisto</a>


**Encore une fois, on se dirige vers Omeka S**. L'outil étant ouvert, nous pouvons l'adapter à l'usage souhaité en particulier car il dispose d'une riche collection de modules et d'une communauté réactive. C'est sur cette base que tout le circuit repose : du dépôt des mémoires par les étudiants à la création de la notice bibliographique. **Il faut penser à la fois à l'outil, mais aussi aux circuits administratifs et pédagogiques** : 

1) On indique en début d'année aux étudiants qu'ils devront déposer la version numérique PDF de leur mémoire sur la plateforme ; 
2) J'envoie un mail aux étudiants en utilisant les listes des promotions pour expliquer la marche à suivre. Dans ce mail, j'indique le lien URL vers le formulaire servant au dépôt des mémoires ; 
3) Les étudiants remplissent le formulaire (titre du mémoire, auteur du mémoire, membres du jury de soutenance, département, date de soutenance, mention du Master, note sur 20, niveau du mémoire [M1 ou M2]) et déposent le PDF de soutenance sur la page ; 
4) Je vérifie les métadonnées du dépôt et corrige si besoin les informations qui pourraient manquer ; 
5) Je valide l'affichage de la notice bibliographique sur la plateforme et je sauvegarde le PDF sur le serveur (un NAS que j'ai installé au sein de l'unité).

Ci-dessous, une capture d'écran du formulaire de dépôt envoyé aux étudiants : 

<img src="/images/depot_1.PNG" alt="Dépôt Omeka S 1" style="width:100%; height:auto;">

Toute le circuit repose donc sur Omeka S et sur un module en particulier : **Collecting** (lien en fin de bidouille). Cette solution est pertinente car elle permet de construire aisément un formulaire et de mettre en place un dépôt de fichiers. En plus, le module fournit un véritable outil en *back-office* qui va vous permettre de suivre, gérer et modérer le dépôt de fichiers et la bascule qui se fait ensuite pour la création de la notice bibliographique. J'ajoute une capture d'écran qui permet de comprendre la construction de formulaire (avec des métadonnées en Dublin Core) : 

<img src="/images/depot_2.PNG" alt="Dépôt Omeka S 2" style="width:100%; height:auto;">

**Vous avez la main sur les propriétés de contenu, les libellés (ce qui s'affiche pour l'utilisateur), l'aspect obligatoire ou non des champs à remplir**. L'onglet "Contenus collectés" vous donne ensuite la possibilité de réviser les dépôts et de gérer l'affichage des notices (Public ou non).

Au final, vous vous retrouvez avec des notices bibliographiques dans une collection Omeka S. Une collection Omeka S sur une page visible. Des PDF sauvegardés sur un serveur NAS (que l'on pourra partager, à la demande, en consultation indirecte). **Et donc un circuit fonctionnel**. Cette solution est améliorable, notamment car il s'agirait, ensuite, de finaliser avec un catalogage systématique sur le SUDOC.

Cette solution présente également un dernier avantage : elle permet de **repérer en amont les mémoires avec une mention "Très Bien"**, et donc, de proposer par la suite aux étudiants et aux enseignants-chercheurs un dépôt complémentaire sur la base DUMAS (Dépôt Universitaire de Mémoires Après Soutenance) géré par le CCSD (Centre pour la Communication Scientifique Directe) en fonction des critères de la composante.

## Pour aller plus loin

* <a href="https://omeka.org/s/modules/Collecting/" target="_blank">Module Collecting</a>
* <a href="https://omeka.org/s/docs/user-manual/modules/collecting/" target="_blank">Documentation du module Collecting</a>