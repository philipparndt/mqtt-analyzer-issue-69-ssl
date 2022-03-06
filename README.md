# mqtt-analyzer-issue-69-ssl

setup to reproduce issue https://github.com/philipparndt/mqtt-analyzer/issues/69

Change the following:

### Your mail address

- `"--certificatesresolvers.myresolver.acme.email=mail@example.com"`

### Your provider settings

see [providers](https://doc.traefik.io/traefik/https/acme/#providers)

- `"--certificatesresolvers.myresolver.acme.dnsChallenge.provider=ionos"`
- `- IONOS_API_KEY=prefix.api_key`

### Your domain name
- ``- "traefik.http.routers.mqtt_websocket.rule=Host(`mqtt.example.com`)"``

## MQTTAnalyzer

<img width="401" alt="image" src="https://user-images.githubusercontent.com/2879650/156918713-ce314227-ef21-4ba0-b96a-fa9631d5b821.png">
