# MYSQL INSTANCE

## Contents:
- Dockerfile
- docker-compose.yml
- .env

### Dockerfile
You dont need to customise this file, you can if you want to use a custom mysql docker image

### docker-compose.yml
> To customise this file you can update the environment values to get started
```yaml
environment:
  - MYSQL_ROOT_PASSWORD=shit@fuckyou
  - MYSQL_DATABASE=fuckthisshit
  - MYSQL_USER=fucksql
  - MYSQL_PASSWORD=yourmomsabitch@1234
```

### To run the docker image use the following command
```git clone git@github.com:ananyakaushik48/mysql.git```
```cd mysql```
```docker-compose up -d```
```bash
mysql -u root -p 'fuckthisshit' -h 127.0.0.1 -P 3306 -D local
```
