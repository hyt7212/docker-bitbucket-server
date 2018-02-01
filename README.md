### Bitbucket Server 5.7.1 for docker

+ Bitbucket Server 5.7.1
+ mysql >= 5.7（Bitbucket Server4.14版本需要mysql <= 5.6）

### 汉化
系统启动成功后进入后台设置导入汉化包

`docker-compose.yml`
```yml
version: '2'
services:
  bitbucket:
    restart: always
    image: ikerlin/bitbucket-server:5.7.1
    ports:
      - 7990:7990
      - 7999:7999
    volumes:
      - ./data:/var/atlassian/application-data/bitbucket
```