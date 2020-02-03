# yansan-integration
[ヤンサンNavi](http://yansan-navi.garaku.work)を構成する以下リポジトリをサブモジュールに含むプロジェクトです。
* [yansan-crawler](https://github.com/U0326/yansan-crawler)
* [yansan-web](https://github.com/U0326/yansan-web)

ヤンサンNaviは、漫画家である山田玲司先生の番組「[山田玲司のヤングサンデー](https://www.youtube.com/channel/UC09D3M_DdLaZMJnZp0v4pLQ)」の動画を整理し、ヤンサンライフを支援することを目的としています。

## 要求事項
Dockerを事前にインストールする必要があります。

## 実行方法
### ローカル
以下手順で実行が可能です。
```
git clone --recursive https://github.com/U0326/yansan-integration.git
cd ./yansan-integration
docker-compose -f docker-compose-local.yml up
```
### 本番環境
注)本番環境では、[こちら](https://github.com/U0326/garaku-proxy)のプロジェクトをフォワードプロキシとして用いています。  
以下手順で実行が可能です。
```
git clone --recursive https://github.com/U0326/yansan-integration.git
cd ./yansan-integration
docker-compose up
```

