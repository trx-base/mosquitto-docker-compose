# mosquitto-docker-compose
A docker compose project for the Mosquitto MQTT broker. 


## Configuration

### Docker Compose
- Copy `env.example` tp `.env` and adapt and adapt environment variables if needed. 

### Mosquitto

- Mosquitto configuration is located at `./config/mosquitto.conf` 
- Configuration manual can be found here: https://mosquitto.org/man/mosquitto-conf-5.html
- Secure web socket connection is enabled by Traefik and is reachable on default https port 443. Example wss://mosquitto.example.com/mqtt


###  whoami

The `whoami` container is needed for LetsEncrypt because it needs to send a simple verification request to the http entry point.