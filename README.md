# Mutual TLS with Nginx and NodeJS

first of all create server.key and server.crt

```bash
openssl req -x509 -nodes -days 9999 -newkey rsa:2048 -keyout server.key -out server.crt
```

we can skip all the question pressing enter

after, we create client.key and client.crt

```bash
openssl req -x509 -nodes -days 9999 -newkey rsa:2048 -keyout client.key -out client.crt
```

we transfer the all certs and keys to server with filezilla
