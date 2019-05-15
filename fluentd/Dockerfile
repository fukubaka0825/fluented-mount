FROM fluent/fluentd

RUN apk add --update --virtual .build-deps sudo build-base ruby-dev \
 && sudo gem install fluentd-plugin-s3 \
 && sudo gem sources --clear-all \
 && apk del .build-deps \
 && rm -rf /var/cache/apk/* /home/fluent/.gem/ruby/2.4.0/cache/*.gem \
 && 
