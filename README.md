# Verification

## Description


#### Previous steps: 
- [Late Classification](https://github.com/alercebroker/late_classification_step)

## Database interactions

### Insert/Update
- Table ` `

## Previous conditions

- Fields of required features.

## Version
- **0.0.1:** 
	- Use of APF.

## Libraries used
- APF
- Numpy
- Pandas

## Environment variables

### Database setup

- `DB_HOST`: Database host for connection.
- `DB_USER`: Database user for read/write (requires these permission).
- `DB_PASSWORD`: Password of user.
- `DB_PORT`: Port connection.
- `DB_NAME`: Name of database.

### Consumer setup

- `CONSUMER_TOPICS`: Some topics. String separated by commas. e.g: `topic_one` or `topic_two,topic_three`
- `CONSUMER_SERVER`: Kafka host with port. e.g: `localhost:9092`
- `CONSUMER_GROUP_ID`: Name for consumer group. e.g: `correction`

### Producer setup

- `PRODUCER_TOPIC`: Name of output topic. e.g: `correction`
- `PRODUCER_SERVER`: Kafka host with port. e.g: `localhost:9092`

### Elasticsearch setup
- `ES_PREFIX`: Enables the indexing of term prefixes to speed up prefix searches. e.g: `ztf_pipeline`
- `ES_NETWORK_HOST`: Elasticsearch host.
- `ES_NETWORK_PORT`: Elasticsearch port.

## Stream

### Input schema
- Output stream of  [`Late Classifier`](https://github.com/alercebroker/late_classification_step#output-schema).

### Output schema
```json
{}
```

## Build docker image


```bash
```

## Run step


**Note:** Use `docker-compose down` for stop all containers.
