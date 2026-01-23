# Ollama and Ollama WebUI

This project has a docker-compose.yml file to start Ollama and Ollama WebUI on your machine.

## Requirements

- Docker

## Setup

Copy the .env.example file to .env and set the MODELS_PATH variable to the path where your Ollama models are stored.

```sh
cp .env.example .env
```

## Run it

```sh
docker-compose up -d
```

## Stop it

```sh
docker-compose down
```

## Using NVIDIA GPU

If you have an NVIDIA GPU and want to use it with Ollama, you can use the provided `docker-compose.nvidia.yml` file. Make sure you have the NVIDIA Container Toolkit installed on your machine.
To start Ollama with NVIDIA GPU support, run:

```sh
docker-compose -f docker-compose.nvidia.yml up -d
```

Make sure to set the `MODELS_PATH` environment variable to the path where your Ollama models are stored before running the command.
