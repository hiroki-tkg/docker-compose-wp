# WordPress開発環境 with Docker Compose

![](https://www.upcloud.com/support/wp-content/uploads/2016/03/wordpress-docker-compose.png)

※ MacでDocker composeを使ったWordPress開発環境  
  
  
## Dockerのインストール
- Docker for Macを落とす  
[https://docs.docker.com/docker-for-mac/install/](https://docs.docker.com/docker-for-mac/install/)
  
  
## Basic


### 始め方


```
git clone git@bitbucket.org:hirokitakagi/docker-compose-wp.git 
mv docker-compose-wp [任意の開発用ディレクトリ名] 
cd [任意の開発用ディレクトリ名]

# 環境git関連削除
rm -rf .git
rm -f .gitignore

# ホストPCで編集できるように、wp-contentを作成
mkdir wp-content

# Docker Compose をデタッチで起動
docker-compose up -d 

```

dockerがちゃんと動けば、以下ですぐにWordPressにアクセスできます。  
`https://localhost:9000`

一瞬でできるし、環境がコードベースなので、差異がありません。すごい。


作成 : `<tkg.japan@gmail.com>`  


