# Proof of Concept Zilla and Kafka's events

Source: https://github.com/aklivity/zilla-examples/tree/main/http.kafka.cache

https://github.com/aklivity/zilla-examples/tree/main/http.kafka.async

https://docs.aklivity.io/zilla/configure-kafka-proxies/rest-proxy

https://docs.aklivity.io/zilla/reference/zilla.json/binding-http-kafka

https://www.aklivity.io/post/bring-your-own-rest-apis-for-apache-kafka

https://github.com/aklivity/zilla-examples/blob/main/http.kafka.async/conf/zilla.json

## Call the events

```
 curl -v http://localhost:8080/events
```

## Start kafka broker and zilla engine

```
docker stack deploy -c stack.yml test --resolve-image never
```

## Stop Kafka broker and Zilla engine

```
docker stack rm test
```
