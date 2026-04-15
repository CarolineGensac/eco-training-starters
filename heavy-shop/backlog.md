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
* **🌱 Bonne pratique d'éco-conception ciblée :** **Permettre aux personnes en situation de handicap ou porteur de déficiences, d'accéder et d'utiliser efficacement le service numérique** ([Source GR491 - Famille UX/UI](https://gr491.isit-europe.org/crit.php?id=4-3026-uxui-au-dela-des-aspects-purement-reglementaires-lanticipation)).
* **📊 KPI associé :** Taux de conformité pour les contrastes et score de satisfaction lors de tests utilisateur en situation de handicap.
* **💻 Repo ou écran concerné :** Page d'accueil, Barre de recherche, Liste de résultats.
* **✅ Critère de réussite :** L'interface est entièrement navigable sans dépendre uniquement de la couleur.
* **⚡ Niveau de priorité :** Haute.

