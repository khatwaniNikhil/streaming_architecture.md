# Streaming mental model
1. think of transforming a batch based use case on stationary/fixed data to real time processing over continous incoming data

# Streaming business use cases
1. ecomm marketplace showing sku ordered count in last N mins in realtime.
    1. need to continously process new events over a kafka cluster in a moving time frame interval and create/update the aggregates and store in redis and expose the same over api.
2. more complex use case/WINDOWING based fraud analysis can be of ecommerce order events as well sub order events(1 or more per order) coming over Kafka cluster and we need to do processing over each (order and corresponding sub order events) coming in a time window.
