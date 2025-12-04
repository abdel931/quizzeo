# quizzeo
Plateforme de quiz multi-rôles (élève, entreprise, admin)
 Rapport de projet – Quizzeo

 Contexte

Le projet Quizzeo a été réalisé dans le cadre d’un besoin client visant à concevoir une plateforme de quiz en ligne. L’objectif principal était de permettre à différents types d’utilisateurs d’interagir avec des questionnaires selon leurs rôles : élève, entreprise, administrateur, et éventuellement école.

 Objectifs du projet

Créer une application web fonctionnelle et sécurisée

Gérer plusieurs rôles utilisateurs avec des droits spécifiques

Permettre la création, la réponse et le suivi de quiz

Assurer la traçabilité du développement via GitHub

 Architecture technique

Langage serveur : PHP (procédural)

Base de données : MySQL

Front-end : HTML, CSS

Versionnement : Git + GitHub

Serveur local : XAMPP / WAMP

 Organisation du projet

src/ : vues, contrôleurs, logique métier

public/ : pages accessibles (login, logout)

assets/ : fichiers CSS, images

db/ : script SQL de la base de données

README.md : documentation technique

 Gestion des rôles

Utilisateur (USER) : répond à un quiz via un lien, consulte ses résultats, modifie son profil

Entreprise (COMPANY) : crée des quiz, consulte les réponses, analyse les résultats

Administrateur (ADMIN) : gère tous les comptes utilisateurs (activation, suppression, création)

 Sécurité

Vérification des rôles via $_SESSION['user']['role']

Redirection automatique selon le rôle

Protection des pages sensibles

Hashage des mots de passe avec password_hash()

 Fonctionnalités principales

Connexion sécurisée

Création de quiz (QCM ou questions libres)

Réponse à un quiz via lien direct

Affichage des résultats et statistiques

Gestion des utilisateurs (admin)

 Suivi GitHub

Dépôt GitHub public avec commits journaliers

Historique traçable avec nom du développeur

Convention de nommage des commits (feat:, fix:, refactor:)

Livrables

Application web fonctionnelle

Dépôt GitHub : [lien à insérer]

Archive .zip avec code source, base de données, documentation


Difficultés surmontées
Séparation des rôles : il a fallu bien réfléchir à la logique de redirection et de sécurisation pour que chaque utilisateur n’accède qu’à ce qui lui est autorisé.

Sécurité des accès : j’ai dû m’assurer que chaque page vérifie le rôle de l’utilisateur, que les données sensibles soient protégées, et que les formulaires soient sécurisés contre les injections SQL.
Présentation PowerPoint pour la soutenance

 Conclusion

Le projet Quizzeo répond aux attentes du client en termes de fonctionnalités, de sécurité et de clarté. Il est prêt à être utilisé et peut évoluer vers des fonctionnalités plus avancées comme une API, une version mobile ou des statistiques enrichies.
