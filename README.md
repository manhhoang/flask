# flask

- [Flask](http://flask.pocoo.org/)
- [Flask-Injector](https://pypi.python.org/pypi/Flask-Injector)
- [Connexion](https://github.com/zalando/connexion) - Connexion is a framework on top of Flask that automagically handles HTTP requests based on OpenAPI 2.0 Specification (formerly known as Swagger Spec) of your API described in YAML format.
- Upload the given images URL to [Amazon S3](https://github.com/boto/boto)
- Send an event to [RabbitMQ](https://github.com/pika/pika) every time a new room has been indexed serializing the payload with Avro.


**Endpoints**:

Swagger: http://localhost:9090/1.0/ui/

|Method|URI|Description| Status |
|------|---|-----------|--------|
| POST | /room | it will receive the room payload, and it will proceed to index it | **Development** |
| PATCH | /room/{id} | this PATCH method will allow us to make changes on the indexed item | Not started |
| DELETE | /room/{id} | this method will remove the room from the index | Not started |
| GET | /room/{id} | this method will return the room data for a given room id | Not started |
| GET | /health-check | This endpoint retuns the state of the service | Not started |

# Running the environment
docker-compose build && docker-compose up -d
