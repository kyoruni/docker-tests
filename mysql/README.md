# docker-tests/mysql
- 作成されるテーブルと初期データ

```sql
mysql> desc pokemons;
+---------+--------------+------+-----+---------+----------------+
| Field   | Type         | Null | Key | Default | Extra          |
+---------+--------------+------+-----+---------+----------------+
| id      | int unsigned | NO   | PRI | NULL    | auto_increment |
| no      | int unsigned | NO   |     | NULL    |                |
| name    | varchar(10)  | NO   |     | NULL    |                |
| species | varchar(10)  | NO   |     | NULL    |                |
| h       | int unsigned | NO   |     | NULL    |                |
| a       | int unsigned | NO   |     | NULL    |                |
| b       | int unsigned | NO   |     | NULL    |                |
| c       | int unsigned | NO   |     | NULL    |                |
| d       | int unsigned | NO   |     | NULL    |                |
| s       | int unsigned | NO   |     | NULL    |                |
+---------+--------------+------+-----+---------+----------------+
10 rows in set (0.00 sec)

mysql> select * from pokemons;
+----+----+-----------------+--------------+----+----+----+----+----+----+
| id | no | name            | species      | h  | a  | b  | c  | d  | s  |
+----+----+-----------------+--------------+----+----+----+----+----+----+
|  1 |  1 | フシギダネ      | たね         | 45 | 49 | 49 | 65 | 65 | 45 |
|  2 |  4 | ヒトカゲ        | とかげ       | 39 | 52 | 43 | 60 | 50 | 65 |
|  3 |  7 | ゼニガメ        | かめのこ     | 44 | 48 | 65 | 50 | 64 | 43 |
|  4 | 25 | ピカチュウ      | ねずみ       | 35 | 55 | 40 | 50 | 50 | 90 |
+----+----+-----------------+--------------+----+----+----+----+----+----+
```