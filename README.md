# Dockerコンテナ内でvueプロジェクトを作成するテンプレート

## Date
2022/04/30

## Ver
Windows10	
WSL	
Docker	
npm 16	
Docker 20.10.14	
Docker Compose 2.4.1	

## 手順

```bash
$ cd ../
$ cp -r VueDockerTemplate Hogeproject
$ cd Hogeproject
$ docker compose up -d
$ docker-compose exec -u $(id -u $USER) app /bin/bash

# vueプロジェクト作成
$ vue create .
# vueサーバー起動
$ npm serve

```