# mysql java
mysql java 学習用

# MySQLへrootでログイン
 $ mysql -u root -p
パスワード:<>
DBの作成
create database company_db;
ユーザー作成
 create user suser@localhost identified with mysql_native_password  by 'spass';
ユーザーに権限を与える
 grant all on company_db.* to suser@localhost;
rootはログアウト
 exit;
新ユーザ(s_user)でログイン
 mysql -u suser -p
パスワード:<>
DBの確認
 show databases;
使用DBの指定
 use company_db;
テーブルの確認
 show tables;
テーブル作成
 create table shain_table(id smallint UNIQUE, name text, sei text, nen smallint, address text);
データ挿入
insert into shain_table(id,name,sei,nen,address) values('100','山田太郎','男','2002','東京都世田谷区');
insert into shain_table(id,name,sei,nen,address) values('101','鈴木義信','男','2003','宮城県仙台市');
insert into shain_table(id,name,sei,nen,address) values('102','佐藤香織','女','2004','福岡県福岡市');
insert into shain_table(id,name,sei,nen,address) values('103','高橋正美','女','2005','福岡県福岡市');
insert into shain_table(id,name,sei,nen,address) values('104','佐藤隆一','男','2003','宮城県仙台市');
insert into shain_table(id,name,sei,nen,address) values('105','小林誠二','男','2002','東京都江東区');
検索
 select * from shain_table;
参考（テーブル削除）
 drop table shain_table;


