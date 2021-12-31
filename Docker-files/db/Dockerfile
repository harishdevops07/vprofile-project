FROM mysql:5.7.25
LABEL "Project"="Vprofile"
LABEL "Author"="Harish"
ENV MYSQL_ROOT_PASSWORD="vprodbpass"
ENV MYSQL_DATABASE="accounts"
# The file init.sql within docker-entrypoint-initdb.d folder will execute as soon as the db container starts running
# and we're adding the db_backup.sql in folder "docker-entrpoint-initdb.d" to initialize the 'accounts' database
ADD db_backup.sql docker-entrypoint-initdb.d/db_backup.sql