# sls_aws_go_mod

Serverless Framework の `aws-go-mod` テンプレートで作成して、  
使いやすい形に整えるところまでおこなった。

Lambda と紐づく API Gateway の API エンドポイントを  
CloudFront の Origin Domain Path に当てるってことをやってみたかったんだけど、  
そこまで出来てない。

CloudFront は us-east-1 にしか存在しないので、serverless.yml を分ける必要がありそうなところが不便そう。


## Requirements

* Node.js 14.x

## Build

```sh
npm i
```

After installing dependencies,

```sh
make build
```

## Check locally

```sh
npx sls invoke local --docker -f hello -d {}
```

## Deploy

```sh
make deploy
```
# sls_aws_go_mod
