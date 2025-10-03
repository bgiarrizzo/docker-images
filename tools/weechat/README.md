# Weechat

WeeChat container based on Debian

## Build

```bash
docker build -t hyweene/weechat:latest -f Containerfile .
```

## Run

```bash
docker run -it --rm -v ${HOME}/.config/weechat:/home/user/.config/weechat hyweene/weechat:latest
```