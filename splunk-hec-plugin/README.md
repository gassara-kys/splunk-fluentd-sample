# splunk-hec-plugin

- ログファイル（アクセスログ） → fluentd → SplunkCloud
- fluent-plugin-splunk-hecを利用してみる
- https://github.com/splunk/fluent-plugin-splunk-hec


## 準備

- 必要な環境変数とかをセット
```bash
$ export SPLUNK_HEC_HOST=http-inputs-<your-domain>.splunkcloud.com
$ export SPLUNK_HEC_PORT=443
$ export SPLUNK_HEC_TOKEN=<your-token>
$ export SPLUNK_HEC_INDEX=<your-index>
```

- 起動
```bash
$ docker-compose build
$ docker-compose up -d
```

## 入力

```
http://localhost/
```


## 出力

```bash
# splunk cloud search
index=<your-index>
```