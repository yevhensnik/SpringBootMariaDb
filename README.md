brew install mariadb

brew services start mariadb

mysql -u root -p


CREATE DATABASE mydatabase;
CREATE USER 'myuser'@'localhost' IDENTIFIED BY 'mypassword';
GRANT ALL PRIVILEGES ON mydatabase.* TO 'myuser'@'localhost';
FLUSH PRIVILEGES;


brew services stop mariadb




### OR DOCKER

docker pull mariadb


docker run -p 3306:3306 -d --name mariadb -eMARIADB_ROOT_PASSWORD=Password123! mariadb

mariadb --host 127.0.0.1 -P 3306 --user root -pPassword123!

CREATE DATABASE springboot_demo;

use springboot_demo 


CREATE TABLE employees (
id BIGINT AUTO_INCREMENT PRIMARY KEY,
first_name VARCHAR(255) NOT NULL,
last_name VARCHAR(255) NOT NULL,
email_address VARCHAR(255) NOT NULL
);

CREATE SEQUENCE employees_seq;


