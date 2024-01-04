# MYSQL INSTANCE

## Contents:
- Dockerfile
- docker-compose.yml
- .env

### Dockerfile
You dont need to customise this file, you can if you want to use a custom mysql docker image

### docker-compose.yml
> To customise this file you can update the environment variables in the yaml file
```yaml
environment:
  - MYSQL_ROOT_PASSWORD=password@1234
  - MYSQL_DATABASE=mysqllocal
  - MYSQL_USER=sqluser
  - MYSQL_PASSWORD=sqluserpass@1234
```

### To run the docker image use the following command
- Clone the repository
```bash
git clone git@github.com:ananyakaushik48/mysql.git
```
- Change directory to target directory
```bash
cd mysql
```
- Run the container locally with docker-compose (hope you have docker installed) 
```bash
docker-compose up -d
```
- To connect to the database from the command line (need to have mysql-client installed)
```bash
mysql -u root -p 'mysqllocal' -h 127.0.0.1 -P 3306 -D local
```
