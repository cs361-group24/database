# Overview

This is the database that powers the web and android verisons of RemoveMyWaste.

# Find something wrong in the database or want to add a new center?

If you have a github account, you can submit issues [here](https://github.com/cs361-group24/database/issues).

Otherwise, you can (anonymously!) submit corrections or updates [here](https://removemywaste.liambeckman.com/issues).

# Development

Pull requests and forks welcome.

## To create database

```sql
CREATE DATABASE MaterialsDB;
USE MaterialsDB;
CREATE USER 'group24'@'localhost' IDENTIFIED BY 'PASSWORD';
GRANT ALL PRIVILEGES ON MaterialsDB.* to 'group24'@'localhost';
```

## To login and update the database

```sh
mysql -u group24 -p MaterialsDB
```

```sql
source database.sql
\q
```
