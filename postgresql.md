# PostgreSQL

## Create a user

```
$ createuser $username
```

then

```
ALTER USER username option;

// e.g.
ALTER USER nobody CREATEDB;

// Try `\h ALTER USER` in psql console for the details.
```

## Delete a user

```
$ dropuser $username
```

## About the default super user

> there will always be a PostgreSQL user account that has the same name as the
> operating system user that started the server, and it also happens that that
> user always has permission to create databases.

http://www.postgresql.org/docs/9.4/interactive/tutorial-createdb.html

## List users

```
\du
```

## List databases

```
$ psql -l
```

or

```
\l
```
