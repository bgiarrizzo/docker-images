# Weechat

WeeChat container

## Build

```bash
docker build -t bgiarrizzo/weechat:latest -f Containerfile .
```

## Run

```bash
docker run -it --rm --name $(whoami)-weechat \
    -v ${HOME}/.config/weechat:/home/user/.config/weechat \
    -v ${HOME}/.local/share/weechat:/home/user/.local/share/weechat \
    -v ${HOME}/.weechat:/home/user/.weechat \
    -v ${HOME}/.cache/weechat:/home/user/.cache/weechat \
    bgiarrizzo/weechat:latest \
    weechat
```