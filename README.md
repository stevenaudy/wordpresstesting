HOW TO START WORDPRESS USING DOCKER-COMPOSE

Command step-by-step :

1. After download this github, go to folder wordpress.
2. Run : docker-compose up -d (it will contain 4 containers : mysqldb, wordpress, webserver, certbot).
3. Check the container status with : docker-compose ps
4. If container certbot return exit 1, it means the problem could be in port 80 & 443 aren't open or the subdomain is not registered (A record).
5. If all containers is up, go to https://stevenwordpress.stevenweb.com (you can change the domain in file nginx.conf and docker-compose.yml on certbot section) it will open wordpress and register couple steps then install wordpress.
6. You will enter admin wordpress webpage.
7. Done.
