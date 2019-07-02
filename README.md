# Container for balena-cli

This repo contains a files for manage containers related to the balena-cli application.

## Usage
Please add your token in a file at:

```
echo "YOUR_BALENA_TOKEN_HERE" > balena_cli_configs/token
```

and add your public and private keys at:

```
cp $PUB_KEY_LOCATION $PRI_KEY_LOCATION ssh-keys
```

Finally, initialize the services:

```bash
(HOST)$ docker-compose run balena-cli bash
(CONTAINER)$ soruce scripts/add-keys.sh
```

Hope it helps.


David Cardozo