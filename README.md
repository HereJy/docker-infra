# docker-infra
Une infrastructure basique constituée d'un nextcloud et d'un kuma derrière un reverse proxy nginx, le https https est fonctionnel et les certificats sont géré par le conteneur acme-companion.

Tous les dossiers sont en chemin relatif afin de permettre une migration plus simple avec la copie du dossier root du projet. 

Ne pas oublier de remplacer le nom de domaine "server.local" par votre nom de domaine et le name@email.com par votre email.

Afin de pouvoir déployer des fichier large, ne pas oublier d'ajouter un fichier de conf dans le volume nginx/conf en y mettant la ligne suivant `client_max_body_size 5G;` en remplaçant 5G par la taille max souhaitée.
