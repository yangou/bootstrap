# bootstrap

Installs all development dependencies in dockerized environment.

# usage

1. Download the latest docker, you will need newer version because it natively mapps the host ports to bridged ports.
2. Once installed newer version, configure it with higher resource limits in `Preferences > Advanced`.

3. clone this repo
4. run `./bootstrap up -d all`

It may ask for permission for the first time.

# tools

Once installed, open a new terminal session, and you get the access to these command line tools:

`.mysql`

`.psql`

`.cqlsh`

`.redis-cli`

(be aware of the prefixing `.`)

# where is the data?

By default, the data is all stored in `./data` , you can change the location by editing `bootstrap` script.

Deleting the data directory will cause lost of dev data.

# logs

```
./bootstrap logs -f    # for all logs
./bootstrap logs -f redis  # for redis only
...

```
