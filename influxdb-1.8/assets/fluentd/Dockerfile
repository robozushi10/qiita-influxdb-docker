FROM fluent/fluentd:v1.13-1

# 次のエラー回避のために root 権限で実行すること.
# You don't have write permissions for the /usr/lib/ruby/gems/2.7.0 directory.
# (ref. https://qiita.com/tamanobi/items/a57f2802c7fd1236ea52)
USER root

RUN gem install fluent-plugin-influxdb

USER fluentd
