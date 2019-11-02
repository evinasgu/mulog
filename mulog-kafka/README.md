# μ/log
[![Clojars Project](https://img.shields.io/clojars/v/com.brunobonacci/mulog.svg)](https://clojars.org/com.brunobonacci/mulog)  [![cljdoc badge](https://cljdoc.org/badge/com.brunobonacci/mulog)](https://cljdoc.org/d/com.brunobonacci/mulog/CURRENT) ![CircleCi](https://img.shields.io/circleci/project/BrunoBonacci/mulog.svg) ![last-commit](https://img.shields.io/github/last-commit/BrunoBonacci/mulog.svg)

![mulog](./doc/mulog.png)

***μ/log*** is a micro-logging library that logs data, not words!

> **μ**, **mu** *(Pronunciation: /mjuː/)* <br/>
> The twelfth letter of the
> Greek alphabet (Μ, μ), often used as a prefix for *mirco-* which is
> 10<sup>-6</sup> in the SI (System of Unis). Lowercase letter "`u`" is often
> substituted for "`μ`" when the Greek character is not typographically
> available.<p/>
> *(source: [https://en.wikipedia.org/wiki/Mu_(letter)](https://en.wikipedia.org/wiki/Mu_(letter)))*
> <br/>


This project contains the `publisher` for [Apache Kafka](https://kafka.apache.org/)


## Usage

Please see [README](../README.md) on main page.

## Testing

``` shell
docker-compose rm -f && docker-compose up -d
docker exec -ti mulog-kafka_kafka_1 /opt/kafka/bin/kafka-console-consumer.sh --bootstrap-server kafka:9092 --topic mulog
```

## License

Copyright © 2019 Bruno Bonacci - Distributed under the [Apache License v2.0](http://www.apache.org/licenses/LICENSE-2.0)