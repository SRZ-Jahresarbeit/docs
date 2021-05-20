```
git clone https://github.com/SRZ-Jahresarbeit/docker.git
docker-compose up -d
```

Now the backend is listening on port `8080` and the mqtt broker is
listening in port `1883`.

to shutdown run:
```
docker-compose down
```

## Updating

1) Take a backup of the `data` directory.
2) run `docker-compose pull` - pulls new docker images form docker hub
3) run `docker-compose down` - shutting down current instance
4) run `docker-compose up -d` - booting up new instance with newly pulled docker images

## Persistance

All relevent data is stored in the `data` directory.

## Testing

### Mqtt
To publish test data to the mqtt broker, you can use:
```
mosquitto_pub -h localhost -p 1883 -t sensor/<sensorId> -m <value>
```

### Swagger
The SwaggerUI is available at [localhost:8080/swagger-ui.html](http://localhost:8080/swagger-ui.html)
