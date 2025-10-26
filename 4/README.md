# Une fois l’archi lancée, vous trouverez le docker debian_psql arrêté. Pourquoi ?
Le client debian_psql est configuré pour utiliser le réseau par défaut de Docker Compose.
Après une connexion réussie à la base de données, le client se termine immédiatement avec un code de sortie 0, indiquant une exécution sans erreur.
Ce comportement permet de confirmer la disponibilité de la base grâce au healthcheck intégré.
