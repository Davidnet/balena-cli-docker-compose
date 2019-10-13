# Container for balena-cli

This repo contains a files for manage devices and applications that are related to the balena-cli application.

## Usage
Please add your token in a file at:

```
echo "YOUR_BALENA_TOKEN_HERE" > balena_cli_configs/token
```

and add your public and private keys at:

```
cp $PUB_KEY_LOCATION $PRI_KEY_LOCATION ssh-keys
```

Finally, initialize the services, sourcing will start a ssh-agent, and balena-cli bash completitions:

```bash
(HOST)$ docker-compose run balena-cli bash
(CONTAINER)$ source scripts/add-keys.sh
```

## Staged Releases submodule
This repo also tracks staged releases [link](https://github.com/balena-io-projects/staged-releases/tree/master) from balena.

Hope it helps.


David Cardozo