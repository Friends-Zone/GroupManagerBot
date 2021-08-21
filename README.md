# GroupManagerBot
This bot will help you to manage your groups and to avoid spam.

# Installation

You can run the bot on your environment or use docker.

## venv (linux)
Configure the `config.toml` file and run
```
./start.sh
```
## Docker
> Use `:latest` for latest published version, you can specify a release or even a branch and commit.
e.g `:master-d1dc0d4`

1. Create a config directory, and create a `config.toml` inside    
    ```bash
    mkdir -p ~/group-manager-config
    cp .config.toml.example ~/group-manager-config/config.toml
    # Configure the bot
    nano ~/group-manager-config/config.toml
    ```
2. Run the docker container, add `-d` to run in the background
    ```bash
    docker run -v ~/group-manager-config:/config \
    ghcr.io/jonatan1609/group-manager-bot:latest
    ```