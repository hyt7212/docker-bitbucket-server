Bitbucket Server 4.14 for docker 汉化版
===
+ Bitbucket Server 4.14
+ mysql <= 5.6

docker-compose.yml
```yml
version: '2'
services:
  bitbucket:
    restart: always
    image: hyt7212/bitbucket-server:4.14
    ports:
      - 7990:7990
      - 7999:7999
    volumes:
      - ./data:/var/atlassian/application-data/bitbucket
```