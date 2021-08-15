# 概要

influxdb 2.0 を使ってコンテナを起動させたときのコード.

ただし、grafana から influxdb に対する接続設定をしたが、
「502 Bad Gateway」エラーが解消できなかった.

なお、influxdb 1.8 で同設定をすれば grafana から influxdb への接続はできたので、
influxdb 2.0 では何か設定が変化しているのかも知れない. 


# 留意点

**次のエラー対策のために、docker-compose.yml の grafana は '472:0' にしている.**

```
GF_PATHS_DATA='/var/lib/grafana' is not writable
```

# 参考にした情報

|URL|
|:--|
|https://www.youtube.com/watch?v=rRKDfU4tmJQ|
|https://github.com/Coac/fluentd-influxdb-grafana|
|https://amemo.hatenablog.jp/entry/2018/07/20/212116|
|https://grafana.com/docs/grafana/latest/installation/docker/#migrate-to-v51-or-later|
|https://qiita.com/tamanobi/items/a57f2802c7fd1236ea52|


