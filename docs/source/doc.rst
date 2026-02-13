Accès au service / Identifiants
==================================================================

Service Counter 5
------------------------------------------------------------------

* URL : https://counter5.openedition.org
* Identifiants Institution : 

  * Nom d'utilisateur et mot de passe identiques à vos identifiants de l'espace Freemium |_| : https://freemium.openedition.org/library

* Identifiants Consortium :

  * Demandez vos identifiants par email à l'adresse |_| : assistance-abonnes@openedition.org

API Sushi
------------------------------------------------------------------

* URL : https://counter5.openedition.org/api
* URL documentation : https://counter5.openedition.org/api/doc
* Identifiants Institution :

  * Nom d'utilisateur (``requestor_id``) : identique à votre nom d'utilisateur de l'espace Freemium |_| : https://freemium.openedition.org/library
  * Clé d'authentification (``api_key``) : vous pouvez obtenir et régénerer votre clé dans l'`espace Freemium <https://freemium.openedition.org/library>`_ |_| : 

    * *Menu API* > *Clé d'authentification*. 
    * Si elle n'est pas générée ou si vous souhaitez la modifier, cliquez sur `Générer une nouvelle clé`.

  * ``customer_id`` : identique au ``requestor_id``.

* Identifiants Consortium :

  * Demandez vos identifiants par email à l'adresse |_| : assistance-abonnes@openedition.org


* Routes API

  * les rapports disponibles au format Counter 5.0 jusqu'à 2024 sont listées ici : https://counter5.openedition.org/api/reports
  * les rapports disponibles au format Counter 5.1 à partir de 2025 sont listées ici: https://counter5.openedition.org/api/r51/reports


Rapports disponibles
==================================================================


.. note:: Les statistiques sont disponibles au format Counter 5.0 jusqu'à 2024 et au format Counter 5.1 à partir de 2025. 

Les différents rapports disponibles sont présentés ci-dessous. Chaque rapport est proposé sous la forme d'un *Master Report*, paramétrable, et de *Standard Views* pour lesquelles les Metric Types, les filtres et les attributs sont présélectionnés.

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

  * Data_Type (5.0 seulement. Au format 5.1, il est systématiquement appliqué)
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
  * Section_Type (Counter 5.0 seulement)
  * YOP
  * Access_Type
  * Access_Method

* **Attributs disponibles** :

  * Data_Type
  * Section_Type (Counter 5.0 seulement)
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

Rapport comptabilisant les accès refusés aux livres en accès restreint non acquis par l'institution. OpenEdition ne limite pas le nombre d'accès simultanés à une ressource. Le Metric_Type Limit_Exceeded ne renvoie donc aucun résultat.

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

Rapport comptabilisant les accès refusés aux revues en accès restreint non acquis par l'institution. OpenEdition ne limite pas le nombre d'accès simultanés à une ressource. Le Metric_Type Limit_Exceeded ne renvoie donc aucun résultat.

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

Rapport comptablisant les accès au texte intégral pour les revues, hors contenus en Open Access, distribué par année de publication.

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

Une *Investigation* est un accès à un élement de contenu en texte intégral OU à des informations présentant cet élément de contenu : les accès aux sommaires de numéros de revues ou de livres, les accès aux résumés des articles sous barrière mobile, les accès aux résumés des chapitres de livres en accès exclusif. Notez que les accès de type *Requests* sont aussi comptabilisés dans les *Investigations*.

Vous pouvez consulter la description complète et illustrée formulée par Counter à l'adresse suivante : https://cop5.countermetrics.org/en/5.1.0.1/03-specifications/03-counter-report-common-attributes-and-elements.html

Total_Item_Investigations et Total_Item_Requests
------------------------------------------------------------------

Les mesures *Total_Item_Investigations* et *Total_Item_Requests* comptabilisent tous les accès à une ressource. Lorsqu’un utilisateur accède à une ressouce (un article, un ouvrage ou un chapitre d’ouvrage...) plusieurs fois au cours d’une :ref:`session utilisateur <user-session>`, chaque accès à cette ressource est comptabilisé dans *Total_Item_**. Les doubles clics éventuels ne sont pas comptabilisés.

Unique_Item_Investigations et Unique_Item_Requests
------------------------------------------------------------------

Les mesures *Unique_Item_Investigations* et *Unique_Item_Requests* comptabilisent le nombre d’éléments de contenu (chapitres, articles, etc.) ayant fait l’objet d’une *Request* ou d'une *Investigation* pris en compte une seule fois par :ref:`session utilisateur <user-session>`.

Unique_Title_Investigations et Unique_Title_Requests
------------------------------------------------------------------

Les mesures *Unique_Title_Investigations* et *Unique_Title_Requests* ne sont applicables que pour les livres. Elles comptabilisent le nombre d'accès uniques à un livre durant une :ref:`session utilisateur <user-session>`. Ainsi, les accès d'un lecteur à 3 chapitres d'un livre en texte intégral au cours d'une session ne seront comptabilisés qu'une fois dans la mesure *Unique_Title_Requests*.

Item et Livres : Différences 5.0 / 5.1
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Les Items sont comptabilisés différement pour le téléchargement d'un livre complet.

**Téléchargement en PDF ou ePub d'un livre de 10 chapitres**

+----------------------+-------------+-------------+
| Mertic               | Counter 5.0 | Counter 5.1 |
+======================+=============+=============+
| Total_Item_Requests  | 1           | 10          |
+----------------------+-------------+-------------+
| Unique_Item_Requests | 1           | 10          |
+----------------------+-------------+-------------+
| Unique_Title_Request | 1           | 1           |
+----------------------+-------------+-------------+


.. _user-session:

Session utilisateur
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Utilisée dans le calcul des mesures *Unique_**, la session d'un utilisateur est définie par 3 critères |_| :

* l'adresse IP de l'utilisateur ;
* le *user-agent* de l'utilisateur ;
* la date + l'heure de la consultation (comprise entre 0 et 23 ; on ne considère pas les minutes et secondes)

Il s'agit d'une approximation de session. En effet, OpenEdition n'enregistre pas les sessions utilisateurs des lecteurs. Cette méthode est valide selon le Code de pratique Counter 5 : `7.3 Counting Unique Items<https://cop5.countermetrics.org/en/5.1.0.1/07-processing/03-counting-unique-items.html>`_.


No_License
------------------------------------------------------------------

Comptabilise les accès refusés à une ressource en accès reservé. Sur OpenEdition, il peut s'agir |_| :

* d'articles de revues sous barrière mobile |_| ;
* d'articles ou de numéros de revues au format PDF ou ePub pour les revues du bouquet Open Access Freemium, pour les institutions non abonnées |_| ;
* de livres ou de chapitre de livres en accès exclusif, non acquis par l'institution |_| ;
* de livres ou de chapitre de livres au format PDF ou ePub en accès exclusif ou Open Access Freemium, non acquis par l'institution.


Limit_Exceeded
------------------------------------------------------------------

OpenEdition ne limite pas le nombre d'accès simultanés à une ressource. Le Metric_Type Limit_Exceeded ne renvoie donc aucun résultat.

Searches_Platform
------------------------------------------------------------------

Recherches effectuées par les utilisateurs et disponible au niveau Platform uniquement.

Sur OpenEdition, cela correspond aux recherches effectuées |_| : 

* sur OpenEdition Search (https://search.openedition.org) |_| ;
* dans le catalogue des revues (https://www.openedition.org/catalogue-journals) |_| ;
* dans le catalogue des livres (https://books.openedition.org/catalogue) |_| ; 
* dans un livre particulier (ex. https://books.openedition.org/oep/8713?q=archive).

API Sushi
==================================================================

La documentation de l'API Sushi est disponible à cette adresse |_| : https://counter5.openedition.org/api/doc.


Counter 5 et Access_Type
==================================================================

La notion d'Access_Type a évolué entre Counter 5.0 et Counter 5.1, en particulier pour la diffusion Freemium.

Counter 5.0 Access_Type et diffusion Freemium
------------------------------------------------------------------

Les revues et les livres publiés en *Open Access Freemium* sont disponibles en libre accès au format HTML et en accès retreint pour les formats PDF et ePub. De ce fait, et suivant les recommandations du *Technical Advisory Group Counter* |_| :

* Les requêtes sur le contenu HTML sont comptabilisées avec un Access_Type='OA_Gold'.
* Les requêtes sur le contenu PDF et ePub sont comptabilisées avec un Access_type='Controlled'.

Une instition abonnée pourra donc observer dans ses rapports Counter 5, pour une même revue, des consultations ayant pour *Access_Type* "OA_Gold" (les consultations aux versions HTML) ET des consultations ayant pour *Access_Type* "Controlled" (les consultations aux versions PDF et ePub).
 
Counter 5.1 access_type et diffusion Freemium
------------------------------------------------------------------

Le code de bonnes pratiques COUNTER exige un seul Access_Type pour chaque élément (Item) et recommande d'utiliser le type d'accès le plus restrictif lorsque différentes parties de l'élément peuvent avoir des règles d'accès différentes. 

Dans le cas de la diffusion en Open access Freemium, toutes les consultations sont donc qualifiées avec Access_Type = Controlled


Tableau récupitualtif des Access_Type
------------------------------------------------------------------

+------------------------------------------+-------------+-------------+
|                                          | Counter 5.0 | Counter 5.1 |
+==========================================+=============+=============+
| **Revue à barrière mobile**                                          |
+------------------------------------------+-------------+-------------+
| Articles sous la barrière mobile         | Controlled  | Controlled  |
+------------------------------------------+-------------+-------------+
| Articles hors barrière mobile            | Controlled  | Open        |
+------------------------------------------+-------------+-------------+
| **Revue en Open Access**                                             |
+------------------------------------------+-------------+-------------+
| Tous les articles                        | OA_Gold     | Open        |
+------------------------------------------+-------------+-------------+
| **Revue en Open Access Freemium**                                    |
+------------------------------------------+-------------+-------------+
| Tous les articles au format HTML         | OA_Gold     | Controlled  |
+------------------------------------------+-------------+-------------+
| Tous les articles au format PDF ou ePub  | Controlled  | Controlled  |
+------------------------------------------+-------------+-------------+
| **Livre en accès exclusif**                                          |
+------------------------------------------+-------------+-------------+
| Tous les chapitres, tous les formats     | OA_Gold     | Open        |
+------------------------------------------+-------------+-------------+
| **Livre en Open Access**                                             |
+------------------------------------------+-------------+-------------+
| Tous les chapitres, tous les formats     | Controlled  | Controlled  |
+------------------------------------------+-------------+-------------+
| **Livre en Open Access Freemuim**                                    |
+------------------------------------------+-------------+-------------+
| Tous les chapitres au format HTML        | OA_Gold     | Controlled  |
+------------------------------------------+-------------+-------------+
| Tous les chapitres au format PDF ou ePub | Controlled  | Controlled  |
+------------------------------------------+-------------+-------------+


Date de disponibilité des rapports et temps de reponse
==================================================================

Dates et durée de disponibilité des rapports
------------------------------------------------------------------

* Les rapports pour un mois donné sont disponibles à partir du 5 du mois suivant.
* Les rapports sont disponibles pour une durée de 2 ans plus l'année courante. Ainsi, les rapports de janvier 2024 et de février 2024 seront disponibles jusqu'au 31/12/2026. Il sera impossible de régénérer les rapports une fois la période de disponibilité écoulée. Les données devront donc avoir été moissonnées préalablement.


Certification
==================================================================

Le service Counter 5 d'OpenEdition a été certifié pour Counter 5.0 par un audit indépendant en 2021.

.. image:: _static/counter-audit-logo.jpg
   :alt: Counter audit passed 
   :target: https://registry.projectcounter.org/platform/9fd59d9f-a669-4756-a4b0-1efeeaf14746
   :width: 250


La certification pour Counter 5.1 est prévue en 2026.


.. |_| unicode:: 0xA0 
   :trim:
