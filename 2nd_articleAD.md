# Article 2: 
## Active Directory : Sa structure physique et pourquoi doit-on le sécuriser ?
<p align="justify">
Dans notre précédent article, nous avons abordé les bases de l’Active Directory en partant de la fonction principale de l’AD, à la définition des types de ressources en évoquant sa structure logique. Nous allons maintenant évoquer la structure physique de l’AD et les raisons pour lesquelles il est indispensable de le sécuriser. 
</p>

## Définissons la structure physique de l’AD

Au niveau de la structure physique, il y a les sites active directory et les contrôleurs de domaine. 
<p align="justify"> 
Les sites Active directory sont très utilisés dans la gestion pour les entreprises qui s’étendent à l’international, qui ont des branches ou des filiales à l’international mais qui regroupent l’ensemble de leur parc informatique sous le même nom de domaine. Les sites regroupent donc physiquement des sous réseaux IP qui sont utilisés pour faire de la réplication via les contrôleurs de domaine. </p>
<p align="justify"> Avant de définir ce qu’est un contrôleur de domaine, donnons un exemple qui permettra de comprendre l’utilité des sites au niveau de l’AD. Imaginons une entreprise du nom de MOB Technologies qui exerce son activité en France et qui a l’ensemble de son parc informatique enregistré sous le nom de domaine MOB.Tech. </p>
<p align="justify"> Suite au rachat d’une très grande entreprise dans son processus de croissance externe, MOB.Tech souhaite enregistrer les actifs informatiques de sa nouvelle acquisition sous son nom de domaine actuel. Les sous réseaux d’adresse IP de l’ensemble du parc international de l’entreprise racheté est connu, de ce fait, regroupé sous un site Active Directory, les administrateurs de MOB Technologies, seront capable de gérer leur nouveau parc via le principal nom de domaine MOB.Tech.
</p>

## Revenons aux contrôleurs de domaines
 
<p align="justify">Un contrôleur de domaine est l’entité principale sinon le serveur sur lequel repose le fonctionnement de l’Active Directory. C’est le serveur qui répond aux demandes d’authentification des utilisateurs et qui contrôle l’ensemble des actions possibles par ceux-ci au niveau du système informatique. C’est un élément très stratégique au niveau de l’AD qui est plébiscité par les hackers car il renferme l’ensemble des données de sécurité qui regroupent les autorisations vis-à-vis du système informatique, l’ensemble des règles de groupe et des noms d’ordinateurs.
</p>

<p align="justify">Chaque domaine doit avoir à minima un contrôleur de domaine. Cependant, pour des besoins de sécurité, il est recommandé d’avoir plus d’un contrôleur de domaine pour chaque site et chaque domaine afin de pouvoir d’une part assurer une redondance logique physique et donc d’autre part de minimiser les dégâts pouvant découler d’une panne au niveau des DC (Contrôleur de domaine ou Domain Controller en anglais).
</p>

<p align="justify">Il faut de même évoquer les rôles FSMO (Flexible Single Master Operations) liés aux contrôleurs de domaines qui sont des tâches AD spécifiques qui ne peuvent être réalisées par tous les contrôleurs de domaines au sein du système informatique. Nous dénombrons 5 rôles FSMO que sont:</p>

  - <p align="justify">Le contrôleur de schéma
  - <p align="justify">Le maître d’attribution de noms de domaine
  - <p align="justify">Le master RID
  - <p align="justify">L’émulateur PDC
  - <p align="justify">L’infrastructure maître 
  
<p align="justify">Nous vous invitons à consulter le lien ici si vous souhaitez obtenir plus d’informations sur ce point. N’hésitez pas à nous le signifier en commentaire si vous souhaitez que nous réalisions un article typique sur les rôles FSMO.
</p>

<p align="justify">Comme promis dans notre précédent article, nous allons procéder rapidement à un petit aparté sur les services AD.</p>

## Alors, qu’est ce que AD DS (Active Directory Domain Services)?

<p align="justify">L’ensemble des services pouvant être fournis par AD sont regroupés sous l’acronyme ADDS et inclut les éléments suivants:</p>

- <p align="justify">Les services de domaines qui permet l’authentification des utilisateurs et leur fournit l’accès au catalogue global (pour la réalisation de requêtes) ,évoqué dans le premier article, regroupant l’ensemble des interactions entre les utilisateurs et les domaines;</p>
 
- <p align="justify">La gestion des droits qui consiste en la protection des données de l’entreprise à travers le contrôle d’accès aux ressources afin de réduire tout risque d’accès non autorisé ou de vol de données sensibles;</p>
 
- <p align="justify">Les services de certificat allant de la création à la surveillance en passant par l’attribution des certificats de sécurité au sein du système informatique. Un certificat de sécurité permet de chiffrer les données échangées au sein d’un système. N’hésitez pas à nous signifier en commentaire si vous souhaitez un article à ce sujet :-) </p>
 
- <p align="justify">Les Lightweight Directory Services qui comme leurs noms l’indiquent permettent la prise en charge d’applications d’annuaire qui utilisent le protocole ouvert et multiplateforme LDAP (Lightweight Directory Access Protocol)</p>
 
- <p align="justify">Les services de Fédérations d’annuaires qui fournissent une authentification unique ou SSO (Single Sign on) pour permettre aux utilisateurs de s’authentifier dans plusieurs applications web au cours d’une seule session.</p>


## Pourquoi est-il important de nos jours de connaître l’AD mais avant tout de le sécuriser ? Citons quelques raisons?

- <p align="justify">AD est utilisé par 99% des entreprises mondiales possédant plus de 1000 employés. Au vu de sa présence dans la majorité des grandes entreprises, tant au niveau professionnel personnel qu’à des perspectives globales de sécurité pour l’entreprise, il est indispensable de maîtriser les bases de l’AD, de savoir comment il fonctionne et de savoir le sécuriser. Nous aborderons certainement des outils connus et les bonnes pratiques vis à vis de l’AD dans nos prochains articles;</p>
 
- <p align="justify">AD est un actif critique pour toute entreprise qui le possède. Comme nous l’avons évoqué précédemment, le piratage d’un AD pourrait conduire à des conséquences dramatiques dans la mesure où accéder à un contrôleur de domaine permettrait à un hacker de de voler l’ensemble des données d’une organisation, de les corrompre, de supprimer des données sensibles et donc de mettre à mal entièrement le bon fonctionnement du business;</p>
 
- <p align="justify">AD est un actif vivant en même temps qu’une entreprise. Sa configuration doit s’aligner avec la vie de l’entreprise et évoluer dans la même cadence. Le départ d’un collaborateur doit impliquer la suppression sinon la désactivation de son compte en même temps que l’apparition de nouvelles mises à jour se doivent d’être réalisées dans les temps pour éviter des conséquences irréversibles pour l’organisme</p>

<p align="justify">Il est donc important pour toutes les entreprises de disposer de personnel qualifié capable de travailler à la sécurisation de leurs AD ainsi que sur la gestion de la sécurité de celui-ci tout le long de son cycle de vie. Nous terminons cette partie en encourageant les jeunes qui débutent dans le domaine à s’y intéresser afin de pouvoir de même se mettre du côté positif de la force dans le but que nous luttions ensemble efficacement sur les vulnérabilités intrinsèques et externes liées à l’AD.</p>
 
<p align="justify">Notre prochain article portera sur les indicateurs d’exposition (IoE) de l’AD et fera un petit tour d’horizon de quelques bonnes pratiques à adopter au niveau de l’AD.</p>

## Sources:

- [Université Tenable](https://www.University.tenable.com)
- [Contrôleur de domaine](https://www.varonis.com/fr/blog/controleur-de-domaine)
- [Roles FSMO](https://docs.microsoft.com/fr-fr/troubleshoot/windows-server/identity/fsmo-roles#:~:text=Le%20titulaire%20du%20r%C3%B4le%20FSMO%20d'infrastructure%20est%20le%20responsable,r%C3%A9f%C3%A9rence%20d'objet%20entre%20domaines.&text=Le%20r%C3%B4le%20Ma%C3%AEtre%20d'infrastructure,de%20catalogue%20global%20(GC).)
- [Certificat de sécurité](https://monentreprisesurle.net/certificat-securite/#:~:text=Qu'est%2Dce%20qu',exemple%2C%20ne%20soient%20pas%20compromises.)

