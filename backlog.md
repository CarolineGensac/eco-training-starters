# Backlog heavy-shop

## Contexte du projet

Le projet represente une boutique catalogue avec listes, recherche, detail produit, panier et checkout simplifie.

## Format attendu

Completer au minimum 3 user stories.

## 📄 User Story 1 : Exploration du service (Visiteur)

* **👤 Contexte :** En tant que **visiteur**, je veux **consulter les trajets disponibles pour un trajet précis**, afin de **décider si le service répond à mes besoins de déplacement futurs.**
* **🎯 Objectif :** Accès à la recherche de trajet simplifiée.
* **🌱 Bonne pratique d'éco-conception ciblée :** **Optimiser le parcours utilisateur RWEB 0005** ([Source GreenIT](https://rweb.greenit.fr/fr/fiches/RWEB_0005-optimiser-le-parcours-utilisateur)).
* **📊 KPI associé :** Nombre moyen d'étapes entre l'arrivée sur la page d'accueil et l'affichage de la première liste de résultats.
* **💻 Repo ou écran concerné :** Page d'accueil, formulaire de recherche.
* **✅ Critère de réussite :** L'affichage de la liste des résultats pour l'itinéraire saisi se fait en **une seule soumission de formulaire** et en **moins de 3 clics** depuis la page d'accueil.
* **⚡ Niveau de priorité :** Moyenne.


## 📄 User Story 2 : Réservation Rapide (Passager Régulier)

* **👤 Contexte :** En tant qu'**utilisateur régulier et passager**, je veux **réserver un trajet rapidement.**
* **🎯 Objectif :** Accès à une liste précise selon les critères du client.
* **🌱 Bonne pratique d'éco-conception ciblée :** **Prioritaire :** Limiter les requêtes HTTP **RWEB 0047** ([Source GreenIT](https://rweb.greenit.fr/fr/fiches/RWEB_0047-limiter-le-nombre-de-requetes-http)).
* **Complémentaires :** Stocker les données statiques localement **RWEB 0064** ([Source GreenIT](https://rweb.greenit.fr/fr/fiches/RWEB_0064-stocker-les-donnees-statiques-localement)) et Éviter les redirections **RWEB 0112** ([Source GreenIT](https://rweb.greenit.fr/fr/fiches/RWEB_0112-eviter-les-redirections)).
* **📊 KPI associé :** Nombre de requêtes HTTP générées par recherche comparé à la version précédente.
* **💻 Repo ou écran concerné :** Page d'accueil, parcours de réservation.
* **✅ Critère de réussite :** La liste des résultats s'affiche après une **unique requête globale** déclenchée par la validation du formulaire, les éléments statiques ne sont pas re-téléchargés et il n'y a aucune redirection.
* **⚡ Niveau de priorité :** Haute.

## 📄 User Story 3 : Publication de trajet avec étapes optimisées

* **👤 Contexte :** En tant que **conducteur**, je veux **publier un trajet en utilisant les suggestions d'étapes**, afin de **trouver plus facilement des passagers sur l'ensemble de mon parcours.**
* **🎯 Objectif :** Augmenter le taux de remplissage des véhicules (optimisation du ratio CO2/passager).
* **🌱 Bonne pratique d'éco-conception ciblée :** **Prioritaire :** Ne charger des données ou du code que lorsque c’est indispensable **RWEB 0046** ([Source GreenIT](https://rweb.greenit.fr/fr/fiches/RWEB_0046-ne-charger-des-donneesdu-code-que-lorsqu-elles-sontil-est-necessaire)).
* **Complémentaire :** Optimiser les requêtes aux bases de données **RWEB 0066** ([Source GreenIT](https://rweb.greenit.fr/fr/fiches/RWEB_0066-optimiser-les-requetes-aux-bases-de-donnees)).
* **📊 KPI associé :** Taux d'occupation moyen par trajet et nombre de requêtes d'autocomplétion par trajet publié.
* **💻 Repo ou écran concerné :** Formulaire "Publier un trajet".
* **✅ Critère de réussite :** 80% des trajets publiés incluent au moins une étape suggérée automatiquement.
* **⚡ Niveau de priorité :** Haute.

## 📄 User Story 4 : Accessibilité de la recherche (Utilisateur Daltonien)

* **👤 Contexte :** En tant qu'**utilisateur daltonien**, je veux **pouvoir identifier clairement les éléments de saisie et les résultats de recherche**, afin de **naviguer sans erreur malgré ma perception limitée des couleurs.**
* **🎯 Objectif :** Garantir une interface inclusive et utilisable efficacement par tous.
* **🌱 Bonne pratique d'éco-conception ciblée :** Permettre aux personnes en situation de handicap ou porteur de déficiences, d'accéder et d'utiliser efficacement le service numérique
([Source GR491 - Famille UX/UI](https://gr491.isit-europe.org/crit.php?id=4-3026-uxui-au-dela-des-aspects-purement-reglementaires-lanticipation)).
* **📊 KPI associé :** Taux de conformité pour les contrastes et score de satisfaction lors de tests utilisateur en situation de handicap.
* **💻 Repo ou écran concerné :** Page d'accueil, Barre de recherche, Liste de résultats.
* **✅ Critère de réussite :** L'interface est entièrement navigable sans dépendre uniquement de la couleur.
* **⚡ Niveau de priorité :** Haute.

## 📄 User Story 5 : Réduction de la consommation de données (Passager mobile)

* **👤 Contexte :** En tant que **utilisateur mobile**, je veux que l’application consomme le moins de données possible afin de **pouvoir rechercher et réserver un trajet même avec une connexion limitée.**
* **🎯 Objectif :** Optimiser l’utilisation de la plateforme sur réseau faible ou mobile.
* **🌱 Bonne pratique d'éco-conception ciblée :** Limiter la volumétrie des échanges
([Source GR491 - Famille Back-end](https://gr491.isit-europe.org/crit.php?id=3-7043-backend-les-operations-realisees-sur-le-front-end)).
* **📊 KPI associé :** Volume moyen de données consommées par recherche de trajet.
* **💻 Repo ou écran concerné :** Page de recherche et résultats de trajets.
* **✅ Critère de réussite :** Aucun chargement inutile et consommation de données optimisée.
* **⚡ Niveau de priorité :** Moyenne.

## 📄 User Story 6 : Amélioration du référencement naturel (Responsable du service)

* **👤 Contexte :** En tant que **responsable du service**, je veux que les pages soient optimisées pour les moteurs de recherche afin de **rendre les trajets visibles et attirer plus d’utilisateurs sur la plateforme.**
* **🎯 Objectif :** Améliorer la visibilité du service sur les moteurs de recherche.
* **🌱 Bonne pratique d'éco-conception ciblée :** Avoir un titre de page et une metadescription pertinents
**RWEB 0011** ([Source GreenIT](https://rweb.greenit.fr/fr/fiches/RWEB_0011-avoir-un-titre-de-page-et-une-metadescription-pertinents-avec-le-contenu-de-la-page))
* **📊 KPI associé :** Nombre d’impressions et de clics issus du trafic organique.
* **💻 Repo ou écran concerné :** Pages de recherche et de résultats.
* **✅ Critère de réussite :** Les pages sont correctement indexées et contiennent les éléments SEO essentiels.
* **⚡ Niveau de priorité :** Moyenne.

## 📄 User Story 7 : Fonctionnement du service avec connexion faible (Utilisateur)

* **👤 Contexte :** En tant que **utilisateur avec une connexion Internet faible ou instable**, je veux pouvoir **utiliser le service sans coupure ni blocage**, afin de **réaliser mes actions essentielles même avec un réseau dégradé**.
* **🎯 Objectif :** Garantir une expérience fluide et continue malgré une faible qualité de connexion.
* **🌱 Bonne pratique d'éco-conception ciblée :** Le service fonctionne-t-il avec des connexions faibles ?
([Source GR491 - Famille Back-end](https://gr491.isit-europe.org/crit.php?id=3-3020-uxui-les-environnements-de-developpement-et-de-tests)).
* **📊 KPI associé :** Taux de succès des actions utilisateur en connexion faible (3G / réseau instable).
* **💻 Repo ou écran concerné :** Toutes les pages du service (authentification, recherche, interaction principale).
* **✅ Critère de réussite :** Les fonctionnalités principales restent accessibles et fonctionnelles même en cas de latence élevée ou de coupure temporaire.
* **⚡ Niveau de priorité :** Haute.

## 📄 User Story 8 : Clarté des informations de trajet (Passager)

* **👤 Contexte :** En tant que **utilisateur**, je veux que les informations d’un trajet soient claires et structurées afin de **comprendre rapidement le prix, l’heure et les points de départ/arrivée sans effort.**
* **🎯 Objectif :** Améliorer la lisibilité des informations de trajet.
* **🌱 Bonne pratique d'éco-conception ciblée :** Favoriser un design simple, épuré et adapté au Web
**RWEB 0012** ([Source GreenIT](https://rweb.greenit.fr/fr/fiches/RWEB_0012-favoriser-un-design-simple-epure-adapte-au-web))
* **📊 KPI associé :** Temps moyen pour comprendre une offre de trajet.
* **💻 Repo ou écran concerné :** Liste et détail des trajets.
* **✅ Critère de réussite :** Les informations essentielles sont visibles immédiatement sans interaction supplémentaire.
* **⚡ Niveau de priorité :** Haute.