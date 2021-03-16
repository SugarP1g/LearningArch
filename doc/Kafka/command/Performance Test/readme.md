## kafka-producer-perf-test

```
usage: producer-performance [-h] --topic TOPIC --num-records NUM-RECORDS [--payload-delimiter PAYLOAD-DELIMITER] --throughput THROUGHPUT [--producer-props PROP-NAME=PROP-VALUE [PROP-NAME=PROP-VALUE ...]]
                            [--producer.config CONFIG-FILE] [--print-metrics] [--transactional-id TRANSACTIONAL-ID] [--transaction-duration-ms TRANSACTION-DURATION] (--record-size RECORD-SIZE |
                            --payload-file PAYLOAD-FILE)

This tool is used to verify the producer performance.

optional arguments:
  -h, --help             show this help message and exit
  --topic TOPIC          produce messages to this topic
  --num-records NUM-RECORDS
                         number of messages to produce
  --payload-delimiter PAYLOAD-DELIMITER
                         provides delimiter to be used when --payload-file is provided. Defaults to new line. Note that this parameter will be ignored if --payload-file is not provided. (default: \n)
  --throughput THROUGHPUT
                         throttle maximum message throughput to *approximately* THROUGHPUT messages/sec. Set this to -1 to disable throttling.
  --producer-props PROP-NAME=PROP-VALUE [PROP-NAME=PROP-VALUE ...]
                         kafka producer related configuration properties like bootstrap.servers,client.id etc. These configs take precedence over those passed via --producer.config.
  --producer.config CONFIG-FILE
                         producer config properties file.
  --print-metrics        print out metrics at the end of the test. (default: false)
  --transactional-id TRANSACTIONAL-ID
                         The transactionalId to use if transaction-duration-ms is > 0. Useful when testing the performance of concurrent transactions. (default: performance-producer-default-transactional-
                         id)
  --transaction-duration-ms TRANSACTION-DURATION
                         The max age of each transaction. The commitTransaction will be called after this time has elapsed. Transactions are only enabled if this value is positive. (default: 0)

  either --record-size or --payload-file must be specified but not both.

  --record-size RECORD-SIZE
                         message size in bytes. Note that you must provide exactly one of --record-size or --payload-file.
  --payload-file PAYLOAD-FILE
                         file to read the message payloads from. This works only for UTF-8 encoded text  files.  Payloads  will  be read from this file and a payload will be randomly selected when sending
                         messages. Note that you must provide exactly one of --record-size or --payload-file.
```

```shell
kafka-producer-perf-test --topic round_topic --num-records 1000 --producer.config producer.properties --print-metrics --throughput 100 --record-size 1024
```
