### Example
connect jdbc where
url="jdbc:mysql://127.0.0.1:3306/db?characterEncoding=utf8&zeroDateTimeBehavior=convertToNull&tinyInt1isBit=false"
and driver="com.mysql.jdbc.Driver"
and user="root"
and password="123456"
as db_1;

load jdbc.`db_1.table_1` as table;