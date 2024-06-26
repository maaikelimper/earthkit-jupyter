# earthkit-jupyter

The repository contains the docker and docker-compose files to run a jupyter-server with the [earthkit](https://earthkit.readthedocs.io/en/latest/) package from ECMWF installed.

## configuration

You need to set a token for the jupyter server. You can do this by setting the `JUPYTER_TOKEN` environment variable in a .env file.

```
JUPYTER_TOKEN=S3cr3tT0k3n
```

## Run the server

1. Install docker and docker-compose
2. Clone this repository
3. Create a .env file defining `JUPYTER_TOKEN` (see above)
4. Run `docker-compose up --build` from the directory where you cloned the repository

## Usage

1. Open a browser and go to `http://localhost:8888`
2. Enter the token you set in the configuration
3. Browse to notebooks and open them