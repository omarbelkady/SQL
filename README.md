### POSTGRES+SQL FUNDAMENTALS ... SU 63526

#### DATA TYPES IN PSQL
- bigint
- bigserial
- bit [n]
- bit varying [ (n) ]
- boolean
- box
- bytea
- character [ (n) ]
- character varying [ (n) ]
- cidr
- circle
- date
- double precision
- inet
- integer
- interval [ fields ] [ (p) ]
- json
- jsonb
- line
- lseg
- macaddr
- macaddr8
- money
- numeric [ (p,s) ]
- path
- pg_len
- point
- polygon
- real
- smallint
- smallserial
- serial
- text
- time
- timestamp
- tsquery
- tsvector
- txid_snapshot
- uid
- xml


#### How To Create A Table
```sql
CREATE TABLE nelanisacobollover(column_name + data_type + constraints)
```



### Creating A Table With Some Constraints
```sql
CREATE TABLE fortran32(
first_name VARCHAR(50),
last_name VARCHAR(50),
loves_cobol BOOLEAN,
day_he_discovered_ftn TIMESTAMP,)
```

### How To Create A Table
```sql
CREATE TABLE cobolfb(id int, first_name VARCHAR(50), last_name VARCHAR(50), gender VARCHAR(6), date_of_birth TIMESTAMP);
```



### Correct Way to Create a Table With Constraints
```sql
CREATE TABLE nelanftn56837(
id BIGSERIAL NOT NULL PRIMARY KEY,
first_name VARCHAR(50) NOT NULL,
last_name VARCHAR(50) NOT NULL,
loves_cobol BOOLEAN NOT NULL,
day_he_discovered_ftn TIMESTAMP NOT NULL,
email VARCHAR(50));
```


### How To Delete A Table
```sql
DROP TABLE tablename;
```

#### In My CASE
```sql
DROP TABLE nelanftn56837;
```

#### BIG SERIAL
- This is an autoincremented number


#### How To Insert Data in Record Without An Email
```sql
INSERT INTO fortran32(first_name, last_name, loves_cobol, day_he_discovered_ftn)
VaLUES("42932", "765262632", `TRUE`, DATE `2016-08-08`);
```

#### How To Insert Data in Record With An Email
```sql
INSERT INTO fortran32(first_name, last_name, loves_cobol, day_he_discovered_ftn, email)
VaLUES("42932", "765262632", `TRUE`, DATE `2016-08-08`, `chensung56837@gmail.com`);
```


#### Sorting Data
```sql
SELECT * from fortran32 ORDER BY first_name ASC;
```


## Operators

#### 1 Is Not Equal To 2
```sql
SELECT 1 <> 2
```

#### Select the very first N people after a certain row thanks to the offset keyword
```sql
SELECT * from fortran32 OFFSET 5 LIMIT 5;
```

### Starting from the nth person query to the very end
```sql
SELECT * from fortran32 OFFSET 5;
```

### List All the Databases
```sql
\l
```

### How To Create A Database(PREFERRED)
```sql
CREATE DATABASE nelanisacobol32;
```

### 2nd Way How To Create A Database
```sql
create database nelanisacobol32;
```


### 1st Way How To Connect To A Database using a username default port is 5432
```sql
psql -h localhost -p 5432 -u nelanslovecs nelanisacobol32;
```

