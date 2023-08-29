SELECT * FROM pg_database;

// Запрос выполнять в конкретной БД
SELECT * FROM pg_tables;

SELECT * FROM pg_user;

CREATE ROLE [user] LOGIN;
CREATE ROLE [user];
DROP ROLE [role_name];
SELECT * FROM pg_roles;
GRANT [role_name] TO [user];
REVOKE [role_name] FROM [user];


ALTER DATABASE emp_db
OWNER TO postgres;

pg_dump -O -
-O | --no-owner
-c
-C
-b
-f

# pg_dump
## Дамп структуры БД
pg_dump -c -C -s [db_name]
-c | --clean
-C | --create
-s | --schema-only

## Дамп только данных

-a | --data-only
-b
-E ENCODING | --encoding=ENCODING

## Дамп с конкретикой
-n SCHEMA | --schema=SCHEMA
-N SCHEMA | --exclude-schema=SCHEMA 
-t TABLE  | --table=TABLE
-T TABLE  | --exclude-table=TABLE 

# pg_dumpall
