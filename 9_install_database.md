run

`sudo apt update && sudo apt install mysql-server`

now run `sudo mysql_secure_installation` select No for validate_plugin install (first question) and then yes for all

now run `sudo mysql` and fire `SELECT user,authentication_string,plugin,host FROM mysql.user;` this query to see users.

now alter root user 

`ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY '';`

and

`FLUSH PRIVILEGES;`

now again check users with `SELECT user,authentication_string,plugin,host FROM mysql.user;` query. 

```
+------------------+-------------------------------------------+-----------------------+-----------+
| user             | authentication_string                     | plugin                | host      |
+------------------+-------------------------------------------+-----------------------+-----------+
| root             |                                           | mysql_native_password | localhost |
+------------------+-------------------------------------------+-----------------------+-----------+
```

Now you can access mysql by `mysql -u root` notice we have remove root password now. 

create `test` database for handy temporary database. `create database test;` to check `show databases;`. 

install extensions for php development and testing `sudo apt-get install php-mysql php-xml sqlite3`
