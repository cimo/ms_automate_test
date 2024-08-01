# Ms_automate_test

Microservice automate test.

Depend from Ms_cronjob (use the volume "ms_cronjob-volume" for share the certificate).

## Installation

1. Write on terminal:

```
docker compose -f docker-compose.yaml --env-file ./env/local.env build --no-cache \
&& docker compose -f docker-compose.yaml --env-file ./env/local.env up --detach --pull "always"
```

2. Execute UI:

Write on the container terminal:

```
npm run execute-ui
```

## Reset

1. Remove this from the root:

    - .cache
    - .config
    - .local
    - .npm
    - .pki
    - .ms_cronjob-volume
    - node_modules
    - package-lock.json
    - certificate/tls.crt
    - certificate/tls.key

2. Follow the "Installation" instructions.

## UI

1. Write on the browser url:

https://localhost:1044/login

## Url

1. /info
2. /login
3. /ui
4. /logout
