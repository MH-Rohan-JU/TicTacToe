## Add Database
Do the following: 
```sql
CREATE DATABASE IF NOT EXISTS tictactoe;

USE tictactoe;

CREATE TABLE IF NOT EXISTS playerInfo (
    ID INT AUTO_INCREMENT PRIMARY KEY,
    Name VARCHAR(255),
    Email VARCHAR(255) UNIQUE,
    Password VARCHAR(255),
    Point INT DEFAULT 0
);
```
## Compile and Run
You can compile and run using intelliJ by adding the dependency "mysql-connector-java.jar" (if it's not added)

Or use this command:
```bash
javac -cp .: file_path/mysql-connector-java.jar Main.java
java -cp .: file_path/mysql-connector-java.jar Main
```
