## docker-compose phpmyadmin
# run docker-compose 
docker-compose up -d

# stops containers and removes containers, network, volumes, and images create by 'up'
# clean up the data of a particular docker-compose stack
docker-compose down -v --rmi all --remove-orphans

# connet phpmyadmin 
http://localhost

## execute docker-compose with bash (command line)
docker exec -it docker-sql_mariadb_1 bash

# create a database user
GRANT ALL PRIVILEGES ON *.* TO 'db_user'@'localhost' INDENTIFIED BY 'pass_user';

# login mysql
mysql -u root -p
enter pass : mypass123
# or
mysql -u db_user -p
enter pass : pass_user


# create database new
CREATE DATABASE name_database;

# show database
SHOW DATABASES;

# choosing a database
USE name_database;

# check database on the chosen database
SELECT database();

# 