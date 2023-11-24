# mysql and java practice

Foobar is a Python library for dealing with word pluralization.

## Installation

use mysql 8.2 and eclipse


## Usage

mysql -u root -p

```sql
create database company_db;
# create user
create user suser@localhost identified with mysql_native_password  by 'spass';
# grant authority user
grant all on company_db.* to suser@localhost;
# logout root
exit;
# new user login suser
mysql -u suser -p
# confirm DB
show databases;
# use db
use company_db;
# table
show tables;
# create table
create table shain_table(id smallint UNIQUE, name text, sei text,
# insert data
insert into shain_table(id,name,sei,nen,address) values('100','山田太郎','男','2002','東京都世田谷区');
# search
select * from shain_table;
# drop
drop table shain_table;
# rename

```

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
