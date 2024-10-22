# FROM mysql:8.0
# ENV MYSQL_ROOT_PASSWORD=ExpenseApp@1
# ADD scripts/*.sql /docker-entrypoint-initdb.d
    ##MYSQL_DATABASE=trasactions \
    ##MYSQL_USER=expesne \
    ##MYSQL_PASSWORD=ExpenseApp@1




FROM mysql:8.0
ENV MYSQL_ROOT_PASSWORD=ExpenseApp@1
RUN groupadd expense && \
    useradd -g expense expense && \
    chown -R expense:expense /var/lib/mysql /var/run/mysql /docker-entrypoint-initdb.d
ADD script/*.sql /docker-entrypont-initdb.d
USER expense