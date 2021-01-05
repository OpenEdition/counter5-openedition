Accès au service / Identifiants
==================================================================

Service Counter 5
------------------------------------------------------------------

* URL : https://counter5.openedition.org
* Identifiants Institution : 

  * nom d'utilisateur et mot de passe identiques à vos identifiants de l'espace Freemium : https://freemium.openedition.org/library

* Identifiants Consortium :

  * Demandez vos identifiants par email à l'adresse : assistance-abonnes@openedition.org

API Sushi
------------------------------------------------------------------

* URL : https://counter5.openedition.org/api
* URL documentation : https://counter5.openedition.org/api/doc
* Identifiants Institution :

  * Nom d'utilisateur (``requestor_id``) : identique à votre nom d'utilisateur de l'espace Freemium : https://freemium.openedition.org/library
  * Clé d'authentification (``api_key``) : vous pouvez obtenir et régénerer votre clé dans l'`espace Freemium <https://freemium.openedition.org/library>`_ : 

    * *Menu API* > *Clé d'authentification*. 
    * Si elle n'est pas générée ou si vous souhaitez la modifier, cliquez sur `Générer une nouvelle clé`.

  * ``customer_id`` : identique au ``requestor_id``.

* Identifiants Consortium :

  * Demandez vos identifiants par email à l'adresse : assistance-abonnes@openedition.org



Rapports disponibles
==================================================================

Les tableaux suivants présentent les différents rapports disponibles. Chaque Rapport est proposé sous la forme d'un *Master Report*, paramétrable, et de *Standard Views* pour lesquelles les Metric Types, les filtres et les attributs sont présélectionnés.

Les *Metric Types* sont les différentes mesures d'usage définies par Counter. Vous trouverez plus bas une description de chacune.

L'utilisation d'un *filtre* dans un Master Report permet de limiter le contenu du rapport à un critère particulier. Par exemple le choix d'un filtre ``YOP=2020`` (*Year Of Publication*) limitera le rapport aux contenus publiés en 2020.

L'utilisation d'un *Attribut* dans un Master Report permet de distribuer chaque métrique selon cet attribut. Par exemple le choix d'un attribut ``YOP`` (`Year Of Publication`) pour un rapport TR renverra les métriques pour chaque type par année de publication.


Platform Reports
------------------------------------------------------------------

PR | Platform Master Report
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Rapport personnalisable résumant l'activité sur l'ensemble de la plateforme. Il est paramétrable (filtres et attributs).

* **Type** : 

  * Master Report

* **Metric Types disponibles** : 

  * Total_Item_Investigations
  * Total_Item_Requests
  * Unique_Item_Investigations
  * Unique_Item_Requests
  * Unique_Title_Investigations
  * Unique_Title_Requests
  * Searches_Platform

* **Filtres disponibles** :

  * Data_Type
  * Access_Method

* **Attributs disponibles** :

  * Data_Type
  * Access_Method

PR_P1 | Platform Usage
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Rapport d'usage de la plateforme OpenEdition distribué par *Metric Type*.

* **Type** : 

  * Standard View

* **Metric Types présélectionnés** : 

  * Total_Item_Requests
  * Unique_Item_Requests
  * Unique_Title_Requests

* **Filtres présélectionnés** :

  * Access_Method=Regular

* **Attributs présélectionnés** :

  * aucun

Title Reports
------------------------------------------------------------------

TR | Title Master Report
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Rapport personnalisable détaillant l'activité pour chaque titre, c'est-à-dire pour chaque livre et chaque revue. Il est paramétrable (filtres et attributs).

* **Type** : 

  * Master Report

* **Metric Types disponibles** : 

  * Total_Item_Investigations
  * Total_Item_Requests
  * Unique_Item_Investigations
  * Unique_Item_Requests
  * Unique_Title_Investigations
  * Unique_Title_Requests
  * No_License
  * Limit_Exceeded

* **Filtres disponibles** :

  * Data_Type
  * Section_Type
  * YOP
  * Access_Type
  * Access_Method

* **Attributs disponibles** :

  * Data_Type
  * Section_Type
  * YOP
  * Access_Type
  * Access_Method



TR_B1 | Book Requests (Excluding OA_Gold)
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Rapports sur l'activité en texte intégral pour les livres, hors contenus en Open Access.

* **Type** : 

  * Standard View

* **Metric Types présélectionnés** : 

  * Total_Item_Requests
  * Unique_Title_Requests

* **Filtres présélectionnés** :

  * Data_Type=Book
  * Access_Type=Controlled
  * Access_Method=Regular

* **Attributs présélectionnés** :

  * YOP

TR_B2 | Book Access Denied
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Rapport comptabilisant les accès refusés aux livres en accès restreint non acquis pas l'institution. OpenEdition ne limite pas le nombre d'accès simultanés à une ressource. Le Metric_Type Limit_Exceeded ne renvoie donc aucun résultat.

* **Type** : 

  * Standard View

* **Metric Types présélectionnés** : 

  * No_License
  * Limit_Exceeded

* **Filtres présélectionnés** :

  * Data_Type=Book
  * Access_Method=Regular

* **Attributs présélectionnés** :

  * YOP

TR_B3 | Book Usage by Access Type
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Rapport portant sur l'utilisation des livres indiquant tous les Metric_Types applicables, distribués par Access_Type (Controlled ou OA_Gold).

* **Type** : 

  * Standard View

* **Metric Types présélectionnés** : 

  * Total_Item_Investigations
  * Total_Item_Requests
  * Unique_Item_Investigations
  * Unique_Item_Requests
  * Unique_Title_Investigations
  * Unique_Title_Requests

* **Filtres présélectionnés** :

  * Data_Type=Book
  * Access_Method=Regular

* **Attributs présélectionnés** :

  * YOP
  * Access_Type


TR_J1 | Journal Requests (Excluding OA_Gold)
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Rapports sur l'activité en texte intégral pour les revues, hors contenus en Open Access.

* **Type** : 

  * Standard View

* **Metric Types présélectionnés** : 

  * Total_Item_Requests
  * Unique_Item_Requests

* **Filtres présélectionnés** :

  * Data_Type=Journal
  * Access_Type=Controlled
  * Access_Method=Regular

* **Attributs présélectionnés** :

  * aucun

TR_J2 | Journal Access Denied
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Rapport comptabilisant les accès refusés aux revues en accès restreint non acquis pas l'institution. OpenEdition ne limite pas le nombre d'accès simultanés à une ressource. Le Metric_Type Limit_Exceeded ne renvoie donc aucun résultat.

* **Type** : 

  * Standard View

* **Metric Types présélectionnés** : 

  * No_License
  * Limit_Exceeded

* **Filtres présélectionnés** :

  * Data_Type=Journal
  * Access_Method=Regular

* **Attributs présélectionnés** :

  * aucun

 
TR_J3 | Journal Usage by Access Type
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Rapport portant sur l'utilisation des revues indiquant tous les Metric_Types applicables, distribués par Access_Type (Controlled ou OA_Gold).

* **Type** : 

  * Standard View

* **Metric Types présélectionnés** : 

  * Total_Item_Investigations
  * Total_Item_Requests
  * Unique_Item_Investigations
  * Unique_Item_Requests

* **Filtres présélectionnés** :

  * Data_Type=Journal
  * Access_Method=Regular

* **Attributs présélectionnés** :

  * Access_Type

  
TR_J4 | Journal Requests by YOP (Excluding OA_Gold)
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Rapport comptablisant les accès au texte intégral pour les revues, hors contenu en Open Access, distribué par année de publication.

* **Type** : 

  * Standard View

* **Metric Types présélectionnés** : 

  * Total_Item_Requests
  * Unique_Item_Requests

* **Filtres présélectionnés** :

  * Data_Type=Journal
  * Access_Type=Controlled
  * Access_Method=Regular

* **Attributs présélectionnés** :

  * YOP

Metric types
==================================================================

Investigations / Requests
------------------------------------------------------------------

La spécification Counter 5 distingue les consultations d'éléments de contenu selon les types *Request* et *Investigation*.

Une *Request* est un accès à un élement de contenu en texte intégral : un article en HTML ou en PDF, un numéro de revue complet en PDF, un chapitre de livre ou un livre complet, en  HTML, PDF ou ePub.

Une *Investigation* est un accès à un élement de contenu en texte intégral OU a des informations présentant cet élément de contenu : les accès aux sommaires de numéros de revues ou de livres, les accès aux résumés des articles sous barrière mobile, les accès aux résumés des chapitres de livres en accès exclusif et tous les accès considérés comme *Investigations*. Notez que les accès de type *Requests* sont aussi comptabilisés dans les *Investigations*.

Vous pouvez consulter la description complète et illustrée formulée par Counter à l'adresse suivante : https://www.projectcounter.org/code-of-practice-five-sections/3-0-technical-specifications/#commonattributes.

Total_Item_Investigations et Total_Item_Requests
------------------------------------------------------------------

Les mesures *Total_Item_Investigations* et *Total_Item_Requests* comptabilisent tous les accès à une ressource. Lorsqu’un utilisateur accède à une ressouce (un article, un ouvrage ou un chapitre d’ouvrage...) plusieurs fois au cours d’une :ref:`session utilisateur <user-session>`, chaque accès à cette ressource est comptabilisé dans *Total_Item_**. Les doubles clics éventuels ne sont pas comptabilisés.

Unique_Item_Investigations et Unique_Item_Requests
------------------------------------------------------------------

Les mesures"*Unique_Item_Investigations* et *Unique_Item_Requests* comptabilisent le nombre d’éléments de contenu (chapitres, articles, etc.) ayant fait l’objet d’une *Request* ou d'une *Investigation* pris en compte une seule fois par :ref:`session utilisateur <user-session>`.

Unique_Title_Investigations et Unique_Title_Requests
------------------------------------------------------------------

Les mesures *Unique_Title_Investigations* et *Unique_Title_Requests* ne sont applicables que pour les livres. Elles comptabilisent le nombre d'accès uniques à un livre durant une :ref:`session utilisateur <user-session>`. Ainsi, les accès d'un lecteur à 3 chapitres d'un livre en texte intégral au cours d'une session ne seront comptabilisés qu'une fois dans la mesure *Unique_Title_Requests*.

.. _user-session:

Session utilisateur
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Utilisée dans le calcul des mesures *Unique_**, la session d'un utilisateur est définie par 3 critères :

* l'adresse IP de l'utilisateur ;
* le *user-agent* de l'utilisateur ;
* l'heure de la consultation.

Elle a une durée d'une heure.


No_License
------------------------------------------------------------------

Comptabilise les accès refusés à une ressource en accès reservé. Sur OpenEdition, il peut s'agir :

* d'articles de revues sous barrière mobile ;
* d'articles ou de numéros de revues au format PDF ou ePub pour les revues du bouquet Open Access Freemium, pour les institutions non abonnées ;
* de livres ou de chapitre de livres en accès exclusifs, non acquis par l'institution ;
* de livres ou de chapitre de livres au format PDF ou ePub en accès exclusifs ou Open Access Freemium, non acquis par l'institution.


Limit_Exceeded
------------------------------------------------------------------

OpenEdition ne limite pas le nombre d'accès simultanés à une ressource. Le Metric_Type *Limit_Exceeded* ne renvoie donc aucun résultat.

Searches_Platform
------------------------------------------------------------------

Recherches effectuées par les utilisateurs et disponible au niveau Platform uniquement.

Sur OpenEdition, cela correspond aus recherches effectuées : 

* sur OpenEdition Search (https://search.openedition.org) ;
* dans le catalogue des revues (https://www.openedition.org/catalogue-journals) ;
* dans le catalogue des livres (https://books.openedition.org/catalogue) ; 
* dans un livre particulier (ex. https://books.openedition.org/oep/8713?query=archive).

API Sushi
==================================================================

La documentation de l'API Sushi est disponible à cette adresse : https://counter5.openedition.org/api/doc.


Counter 5 et contenus Freemium
==================================================================

Les revues et les livres publiés en *Open Access Freemium* sont disponibles en libre accès au format HTML et en accès retreint pour les formats PDF et ePub. De ce fait, et suivant les recommandations du *Technical Advisory Group Counter* :

* Les requêtes sur le contenu HTML sont comptabilisées avec un Access_Type="OA_Gold".
* Les requêtes sur le contenu PDF et ePub sont comptabilisées avec un Access_type="Controlled".

Une instition abonnée pourra donc observer dans ses rapports Counter 5, pour une même revue, des consultations ayant pour *Access_Type* "OA_Gold" (les consultations aux versions HTML) ET des consultations ayant pour *Access_Type* "Controlled" (les consultations aux versions PDF et ePub).
 

Date de disponibilité des rapports et temps de reponse
==================================================================

Dates et durée de disponibilité des rapports
------------------------------------------------------------------

* Les statistiques Counter 5 pour un mois donné sont disponibles à partir du 5 du mois suivant.
* Les rapports sont disponibles pour une durée de 2 ans plus l'année courante. Ainsi, les rapports de janvier 2021 et de février 2021 seront disponibles jusqu'au 31/12/2023. 
* Les rapports sont disponibles à compter du mois de juillet 2020.

Temps de réponse et mise en cache
------------------------------------------------------------------

Ce service traite d'importants volumes de données et peut de ce fait nécessiter des temps de calcul non négligeables.

Si le temps de calcul d'un rapport dépasse la limite définie par Counter 5 (120 sec.), l'application renverra un avertissement vous invitant à ré-exécuter votre requête. Dans ce cas, le calcul du rapport continue en arrière plan et lorsque vous ré-exécuterez la demande après quelques minutes, l'application disposera du rapport pré-calculé et pourra vous le renvoyer. 

Ce comportement s'applique également à Sushi qui renverra l'exception 1011 définie par Counter 5 : https://www.projectcounter.org/appendix-f-handling-errors-exceptions/

Le temps de génération dépend de la complexité et la taille du rapport demandé, notamment l'utilisation simultanée de plusieurs attributs, l'utilisation de plage temporelles de plusieurs mois, les rapports pour les consortia.

Pour faciliter l'utilisation de l'application, les rapports des derniers mois (4 derniers mois environ) sont pré-caclulés (en mémoire cache). Le temps de reponse est de ce fait beaucoup amélioré pour les mois récents. Pour les rapports plus anciens, il faut faire preuve de patience.


