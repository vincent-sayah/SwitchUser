# SwitchUser SSI - ILIAS 10

Version corrigée et durcie du plugin SwitchUser.

## Principales corrections SSI

- abandon des actions de bascule en GET au profit d'actions POST ;
- ajout d'un jeton CSRF côté session ;
- journalisation des événements sensibles ;
- régénération d'identifiant de session au début et à la fin de la bascule ;
- refus de basculer vers un compte administrateur ;
- suppression des fichiers de sauvegarde `.bak` ;
- validation stricte des identifiants utilisateurs ;
- bannière persistante avec bouton de retour sécurisé.

## Emplacement

Installer le dossier dans :

`public/Customizing/global/plugins/Services/UIComponent/UserInterfaceHook/SwitchUser`

## Accès

- depuis la configuration du plugin dans l'administration ILIAS ;
- via `goto.php?target=swus_open` pour la page de recherche ;
- les actions de démarrage et d'arrêt de bascule exigent un POST valide.

## Points d'attention

Cette version est fournie sur la base d'une revue de code et d'un durcissement défensif. Elle n'a pas été exécutée ici sur une instance ILIAS réelle. Un test sur préproduction reste indispensable.


## 2.1.0

- Added a direct SwitchUser quick-access entry in the ILIAS side menu for administrators.


## 2.1.1
- enregistrement effectif du provider Global Screen du menu latéral
- ajout d’un accès rapide visible dans l’interface pour les administrateurs
