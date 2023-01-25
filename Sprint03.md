# Sprint 3

## Nouveau à modéliser (sur la base existante des sprints 1 et 2)

* Le chef de cuisine aura dorénavant les possibilités suivantes :
    * Alerte hygiène :
        * un système permettant de suivre la chaîne du froid (*cold chain monitoring*) a été interfacé avec notre plateforme de gestion du restaurant.
        * le chef de cusine reçoit des alertes en lien avec un problème d'hygiène (*get cold chain alert*)
        * il peut également recevoir ces alertes sur ton téléphone mobile (*get cold chain alert by mobile phone*)
        * écrire les menus des jours suivants (*write menu*).

* Le responsable de salle aura dorénavant les possibilités suivantes :
    * Carte des vins :
        * Prendre la commande des vin (*take wine order*).
        * La commande des vins ne peut être réalisée que si la majorité du client est validée (check majority). C'est le serveur qui est responsable de cette vérification avant de valider la commande du repas.
        * Les clients ne sont pas obligés de commander du vin, mais par contre obligé de commander un repas pour avoir du vin.

## Diagramme de cas d'utilisation

Critères d'évaluation :
* vous livrez une mise à jour du diagramme de cas d'utilisation existant
* le système actuel (sprint 1) n'est pas déstabilisé (ne rien modifier, ni supprimer)
* les éléments qui peuvent être ajoutés:
  * 5 cas d'utilisation
  * 2 acteurs "système" externes
  * 2 extends
  * 1 include.

## Diagramme de classes

Complément d'informations (pour simplifier la modélisation):
* les méthodes que vous ajoutez retournent "void"
* l'attribut "orders" de la classe waiter doit désormais être accessible en direct (sans getters ni setters) au "HeadWaiter".
* une commande de vin est intégrée à une commande "de base"
* le chef peut modifier s'il désire ou non être notifié sur ton téléphone mobile (cold chain alert)

Critères d'évaluation
* vous livrez une mise à jour du diagramme de classe existant
* le système actuel (sprints 1 et 2) n'est pas déstabilisé. Des attributs ou méthodes peuvent bien entendus être ajoutés aux classes.
* les éléments qui peuvent être ajoutés :
  * 1 nouvelle classe
  * 5 nouvelles méthodes
  * 2 attributs privés
  * Une relation de type composition
  * Une relation de type usage.