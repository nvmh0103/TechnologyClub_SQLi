FROM handsonsecurity/seed-server:apache-php

ARG WWWDir=/var/www/SQL_Injection

COPY Code $WWWDir
RUN rm -rf /etc/apache2/sites-enabled/000-default.conf
COPY apache_sql_injection.conf  /etc/apache2/sites-available
RUN  a2ensite apache_sql_injection.conf
EXPOSE 80



