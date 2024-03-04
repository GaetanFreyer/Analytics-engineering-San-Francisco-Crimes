## Analyse de données sur les crimes à San Francisco
Ce projet consiste à analyser les données sur les crimes signalés à San Francisco entre 2003 et 2021. Les données ont été collectées à partir du site web du département de police de San Francisco et stockées dans une base de données PostgreSQL. Les données ont ensuite été analysées à l'aide de Python et de bibliothèques telles que pandas, numpy, matplotlib et seaborn. Enfin, les résultats ont été visualisés à l'aide de Power BI.

## Installation
Pour exécuter ce projet, vous aurez besoin des éléments suivants :

Docker
Python 3.12
Power BI Desktop

Suivez les étapes suivantes pour installer et exécuter le projet :

Clonez ce dépôt Git sur votre ordinateur local.
Ouvrez un terminal et accédez au répertoire du projet.
Créez un fichier .env à la racine du projet et ajoutez les variables d'environnement suivantes :

POSTGRES_USER=<votre nom d'utilisateur PostgreSQL>
POSTGRES_PASSWORD=<votre mot de passe PostgreSQL>
POSTGRES_DB=<le nom de votre base de données PostgreSQL>
POSTGRES_HOST=<l'adresse IP de votre conteneur PostgreSQL>
POSTGRES_PORT=<le port de votre conteneur PostgreSQL>
Exécutez la commande docker-compose up pour démarrer les conteneurs Docker.
Ouvrez un navigateur web et accédez à l'adresse http://localhost:8888 pour accéder à Jupyter Notebook.
Ouvrez le notebook sf_crime_analysis.ipynb et suivez les instructions pour exécuter le code.
Ouvrez Power BI Desktop et connectez-vous à la base de données PostgreSQL à l'aide des informations de connexion spécifiées dans le fichier .env.
Ouvrez le fichier sf_crime_dashboard.pbix et actualisez les données pour afficher les résultats.

## Résultats

Les résultats de l'analyse ont révélé que :

Les vols sont le type de crime le plus fréquent à San Francisco, représentant environ 40 % de tous les crimes signalés.
Les crimes sont plus fréquents dans les districts de Mission, Tenderloin et Southern.
Les crimes sont plus fréquents le samedi et le dimanche, et moins fréquents le mercredi.
Les crimes sont plus fréquents pendant les heures de pointe, entre 12h00 et 18h00.
Une régression linéaire multiple a été utilisée pour prédire le nombre de crimes signalés en fonction de plusieurs variables, telles que le jour de la semaine, l'heure et le district. Le modèle a obtenu un coefficient de détermination de 0,46.
Conclusion
Ce projet a permis d'explorer les données sur les crimes à San Francisco et de révéler des tendances intéressantes. Les résultats peuvent être utilisés pour aider les forces de l'ordre à allouer leurs ressources de manière plus efficace et à réduire le nombre de crimes dans la ville.

## Crédits
Ce projet a été réalisé par Gaëtan FREYER en utilisant les données du département de police de San Francisco. Le code source est disponible sur GitHub sous licence MIT.