# Backup

For SQL Databases, you will find backup in a couple of formats.

## Using SQL file

If you have as an `SQL` file, then to install it to your server, for [MySQL]() and [MariaDB](), you will log into your server and source the `SQL` file.

```bash
mariabd -u username -p password # log into the server
```

After logging in, create a database and source your file. You can include the absolute path if the file is in a different directory.

Use `pwd` to know your current working directory.

```bash
\! pwd
```

```sql
CREATE DATABASE database_name;
USE database_name;
SOURCE backup.sql; -- You can also provide the absolute path of the file
```
