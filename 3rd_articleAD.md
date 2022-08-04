# Article 3
## Active Directory : Qu’est ce que les IoE AD et quelques bonnes pratiques au niveau de l’AD

<p align="justify"> Dans notre précédent article, nous avions parlé de la structure physique de l’AD et des raisons pour lesquelles les entreprises devraient prendre à cœur la sécurité de l’AD. Avant de nous orienter vers les procédés des hackers en phase de piratage, nous faisons un tour rapidement sur les indicateurs d’expositions et proposons quelques bonnes pratiques intéressantes.</p>
 
## Alors, définissons ce que représentent les indicateurs d’exposition.
 
<p align="justify"> Les indicateurs d’exposition permettent de s’assurer que les infrastructures ne puissent pas être exploitées par des attaquants afin d’obtenir des privilèges d’administrateur. Ils représentent donc l’ensemble des vecteurs d’attaques possibles pour un attaquant afin de pouvoir s’insérer dans le système d’une organisation cible.</p>

<p align="justify"> Il est important pour toute organisation qui se respecte d’identifier ces vecteurs d’exposition et de pouvoir attribuer un niveau de faisabilité de l’exploitation de la vulnérabilité afin que les entreprises puissent s’organiser et identifier leurs priorités vis-à-vis de leurs faiblesses identifiées. Si nous souhaitons faire un lien avec la sécurité fonctionnelle, l’on évoquera l’analyse des risques qui est très importante dans le processus de planification, et plus globalement de gouvernance appliquée dans maintes entreprises de nos jours.</p>

<p align="justify"> L’identification des IoE est donc une “sorte” de gestion de risques cyber avec premièrement l’identification des vulnérabilités applicables aux actifs de l’organisme, l’appréciation de celles-ci par rapport à une échelle définie de vraisemblance et de gravité afin de pouvoir découler sur un niveau de criticité qui nous permettra de définir le plan d’actions le plus adapté aux réalités du système informatique.</p>

## Comment doit-on procéder pour déterminer ces IoE ?
 
<p align="justify"> Plusieurs facteurs doivent être considérés pour se faire mais il faut retenir que tout événement du système informatique qui permettrait d’accéder à un actif critique de l’organisme est un IoE.

Observons ensemble la nuance à travers l’exemple suivant:</p>

- <p align="justify"> Un changement ou une modification inattendue des règles du firewall d’une entreprise est un événement dans le SI
  
- <p align="justify"> Un changement ou une modification inattendue des règles du firewall d’une entreprise qui donne accès à une application métier importante d’une organisation et par la suite à un compte administrateur du système est un IoE.

<p align="justify"> Vous l’avez compris, les IoE ne sont pas intrinsèquement un concept purement AD mais quel lien faisons nous avec l’AD. Il faut dire que nous entendons par IoE AD toute action usant d’une vulnérabilité qui permettrait à un attaquant d’accéder à des ressources critiques de l’architecture AD. </p>

## Mais quels sont les différents types d’IoE AD ?

<p align="justify"> Nous distinguons trois types d’IoE AD que sont:</p>

  - <p align="justify">Les IoE liés aux montées en privilèges

<p align="justify"> Il s’agit ici des indicateurs qui garantissent que l’AD réduit au maximum l’ensemble des vecteurs exploitables par les hackers dans la réalisation de montée en privilège. Une montée en privilège consiste en un changement de droit d’accès aux ressources au sein d’un système.</p>
 
  - <p align="justify">Les IoE liés aux techniques de persistance
  
<p align="justify"> Il s’agit ici de s’assurer que le système ne présente pas de portes dérobées en son sein ou que des techniques de persistance aient été réalisées afin de permettre aux hackers de se rendre comme ils le souhaitent dans le système informatique. Une stratégie de sécurité efficace doit être déployée afin de réduire les risques évoqués.</p>

<p align="justify">Pour rappel, une porte dérobée est un accès tenu secret vis-à-vis de l'utilisateur légitime aux données contenues dans un logiciel ou sur un matériel.</p>

  - <p align="justify">Les IoE liés aux modèles de sécurité dangereux

<p align="justify">Il s’agit ici des indicateurs qui garantissent que l’AD implémente les stratégies de sécurité recommandées afin que les systèmes d’informations puissent être renforcés contre les cyberattaques actuelles.</p>

<p align="justify">Toute entreprise qui souhaite gérer efficacement son AD se doit de bien identifier et gérer leus IoE. Il existe des menaces propres à l’AD mais nous les évoquerons dans les articles à venir :-). Orientons nous dès à présent vers quelques bonnes pratiques de l’AD.</p>

## Bonnes pratiques AD

<p align="justify"> Comme évoqué dans l’article précédent, l’AD est un actif vivant autant qu’une entreprise. De ce fait, l’une des meilleures pratiques de sécurité consiste à examiner régulièrement et de manière proactive les configurations de l’AD et sa conformité vis-à-vis des recommandations globales. Des outils et solutions plug and play existent pour la gestion proactive de l’AD dans les organisations. N’hésitez pas à nous faire savoir si vous souhaitez que l’on vous propose ce type de contenu.</p>

<p align="justify"> En ce qui concerne l’AD, de façon générale, il est important de protéger les comptes de service, limiter le nombre des administrateurs dans le système et réduire les tâches programmées au sein de l’AD. Néanmoins, nous souhaitons vous proposer les 7 bonnes pratiques qui ont été identifiées dans la formation TCSA AD de Tenable que nous avons trouvés particulièrement intéressantes :</p>
 
  - <p align="justify"> Examiner et modifier les paramètres de sécurité par défaut
<p align="justify">Après avoir installé AD, il est essentiel de revoir la configuration de la sécurité et de la mettre à jour en fonction des besoins de l'entreprise. Il y a des outils qui permettent de faire du monitoring de la configuration de l’AD et de présenter les manquements qui y sont présents.</p>

  - <p align="justify"> Mettre en œuvre les principes du moindre privilège dans les rôles et les groupes d'AD
<p align="justify"> Il est intéressant de passer en revue toutes les autorisations nécessaires pour les données et les applications pour tous les rôles des employés dans l'organisation en appliquant le principe du moindre privilège. Ce principe consiste à restreindre les droits d'accès des utilisateurs, des comptes et des processus informatiques aux seules ressources absolument nécessaires à l'exécution d'activités courantes et légitimes. Cette pratique est très recommandée surtout qu’un système n’est jamais totalement intrusion-proof.</p> 

  - <p align="justify">Contrôler les privilèges d'administration AD et limiter les comptes d'utilisateurs du domaine
<p align="justify">Il est important de passer soigneusement en revue l'ensemble du personnel informatique et de n’accorder les privilèges d'administration et l'accès aux superutilisateurs qu'aux personnes qui en ont absolument besoin pour remplir leur rôle. Ce point rejoint un peu celui évoqué plus haut mais avec une attention particulière sur les comptes sensibles.</p> 

  - <p align="justify">Utiliser l'audit et l'alerte Windows en temps réel
<p align="justify">Il faut effectuer des rapports sur les tentatives d'accès inhabituelles et signalez tout accès provenant de l'intérieur ou de l'extérieur de l'organisation. Ces rapports pourront rentrer dans le cadre de la mise en place d’une procédure de gestion d’incidents donc d’amélioration continue qui accompagnera les différents états du cycle de vie de l’AD.</p> 
 
  - <p align="justify">Assurer la sauvegarde et la récupération d'Active Directory
<p align="justify">La sauvegarde régulière de la configuration et du répertoire AD doit être réalisée. Il faut mettre en place des processus de reprise après sinistre pour permettre une récupération rapide en cas d'atteinte à l'intégrité de l'AD. Ces bases de configuration doivent faire partie intégrante des Plan de Reprises d’Activité au vu de l’importance des données se trouvant au niveau de l’AD.</p> 

  - <p align="justify">Corrigez régulièrement toutes les vulnérabilités
<p align="justify">Il faut une équipe en place compétente afin d’assurer un processus de correction et de maintenance rapide, efficace et efficient pour l’AD et les autres failles détectées sur le système d’information.</p> 

  - <p align="justify"Centraliser et automatiser
<p align="justify">La centralisation de l'ensemble des examens, des rapports, des contrôles et de l'administration en un seul endroit est indispensable, et il faut rechercher des outils capables de fournir des interactions systèmes automatisées pour l'émission d'alertes et l'aide à la résolution rapide de problème. Des solutions existantes de centralisation et services managés existent et n’hésitez pas, comme nous l'évoquions souvent, à signifier en commentaire si vous souhaitez que nous fassions typiques sur ce genre de solutions.

<p align="justify">En suivant ces bonnes pratiques, vous réduisez assurément l’ensemble des vecteurs d’attaques possibles vers votre environnement AD. Et vous, quelles sont les bonnes pratiques que vous appliquez dans vos entreprises respectives ? Signifiez les en commentaire pour le partage d’expérience.
 
<p align="justify">Maintenant que l’AD est connu, son vocabulaire, sa structure ainsi que ses bonnes pratiques générales de gestion, nous allons dans notre prochain article aborder les différentes étapes de compromission de l’AD d’un point de vue Hacking.</p> 
 
## Sources:

- [Université Tenable (TCSA)](https://University.tenable.com)
  
- [Porte dérobée](https://www.cnil.fr/fr/definition/porte-derobee-ou-backdoor#:~:text=Le%20principe%20de%20la%20mise,logiciel%20ou%20sur%20un%20mat%C3%A9riel.) 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
