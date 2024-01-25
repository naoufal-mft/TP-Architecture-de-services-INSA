# TP-Architecture-de-services-INSA
Ce projet Talend repose sur l'Enterprise Service Bus (ESB) de Talend et propose trois flux distincts pour des opérations spécifiques :

# Flux 1 - Intégration de fichiers CSV dans la base de données
Le premier flux a pour objectif de consommer un ou plusieurs fichiers au format CSV correctement structurés. Ces fichiers seront placés dans un dossier dédié, et le flux permettra d'intégrer directement les utilisateurs extraits de ces fichiers dans la base de données. Ce flux constitue une opération d'intégration de données entre un système de fichiers et une base de données.

# Flux 2 - API REST pour l'insertion d'utilisateurs
Le deuxième flux expose une API REST gérée par un verbe POST. Cette API permet de recevoir des utilisateurs au format JSON dans le corps de la requête. Les données reçues sont ensuite intégrées directement dans la base de données des utilisateurs. Cela offre une méthode simple et flexible pour ajouter de nouveaux utilisateurs à la base de données.

# Flux 3 - Service Web SOAP pour l'interrogation de la base de données
Le troisième connecteur implémente un service Web de type SOAP. Ce service permet d'interroger la base de données des utilisateurs et de récupérer à la demande un utilisateur en fonction de son numéro ou de son nom. Cette fonctionnalité offre une approche efficace pour obtenir des informations spécifiques sur les utilisateurs stockés dans la base de données.
