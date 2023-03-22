### Usage
----

Install Packages
- yarn install

Up RabbitMQ with docker-compose
- docker-compose up -d

Start Application
- yarn start:dev
    
Start Worker Consumer
- yarn start: dev workers

---

Endpoint Sum [Sync]
```
curl --location 'http://localhost:3000/sum' \
--header 'Content-Type: application/json' \
--data '{
    "data": [9,10]
}'
```


Endpoint Multiply [Async]
```
curl --location 'http://localhost:3000/multiply_by_two' \
--header 'Content-Type: application/json' \
--data '{
    "data": 3
}'
```
