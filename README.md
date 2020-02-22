# yansan-integration
[ヤンサンNavi](http://yansan-navi.garaku.work)を構成する以下リポジトリをサブモジュールに含むプロジェクトです。
* [yansan-crawler](https://github.com/U0326/yansan-crawler)
* [yansan-web](https://github.com/U0326/yansan-web)

ヤンサンNaviは、漫画家である山田玲司先生の番組「[山田玲司のヤングサンデー](https://www.youtube.com/channel/UC09D3M_DdLaZMJnZp0v4pLQ)」の動画を整理し、ヤンサンライフを支援することを目的としています。

## 要求事項
Dockerを事前にインストールする必要があります。

## ローカルでの実行方法
```
git clone --recursive https://github.com/U0326/yansan-integration.git
cd ./yansan-integration
docker-compose -f docker-compose-local.yml up
```

## 本番環境へのデプロイ
CircleCIを用いており、以下形式のタグを発行すると自動で本番環境のへのデプロイが行われます。
```
^v[0-9]+(\.[0-9]+)*
```
CircleCIの設定詳細は[こちら](./.circleci/config.yml)をご覧ください。
