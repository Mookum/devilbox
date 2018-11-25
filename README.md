## DevilBox
1. git clone https://github.com/cytopia/devilbox
2. cd devilbox
3. cp env-example .env
4. sudo vim .env
5. change HTTPD_DOCROOT_DIR=htdocs  to HTTPD_DOCROOT_DIR=web
6. change TLD_SUFFIX=loc to TLD_SUFFIX=local
7. start container with docker-compose up -d
8. enter container with ./shell.sh
9. setup drupal project with composer create-project drupal-composer/drupal-project:8.x-dev yourprojectName --stability dev --no-interaction
10. browse to http://localhost/vhosts.php
11. add DNS Host to hosts with sudo vim /etc/hosts
12. browse to localhost via tools phpMyAdmin create database (root no pasword)
13. create database (utf8_general__ci)
14. Drupal install (Host = 127.0.0.1)
15. enter container with ./shell.sh
