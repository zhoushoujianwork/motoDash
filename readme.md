## 1. start

### DB

    docker run -d -p 3306:3306 -e MYSQL_ROOT_PASSWORD=motobox --name mariadb mariadb:10.2.40

    GRANT ALL PRIVILEGES ON *.* TO 'root'@'%' WITH GRANT OPTION; 

    create database motodashdb;

    mysql -u root -h 192.168.1.40 -P 3306 -pmotobox

    mysql -u root -h 192.168.1.40 -P 3306 -pmotobox < Database/data.sql 


### 其他

打包项目依赖
```
yum install -y make gcc mysql-devel
pip3 freeze >requirements.txt

```

<!-- 容器启动web -->

