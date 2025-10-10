# neomutt

neomutt container

## Build

```bash
docker build -t bgiarrizzo/neomutt:latest -f Containerfile .
```

## Run

```bash
docker run -it --rm --name $(whoami)-neomutt \
    -v ${HOME}/.config/mutt:/home/user/.config/mutt \
    -v ${HOME}/.local/share/mutt:/home/user/.local/share/mutt \
    -v ${HOME}/.local/state/mutt:/home/user/.local/state/mutt \
    -v ${HOME}/.mutt:/home/user/.mutt \
    -v ${HOME}/.cache/mutt:/home/user/.cache/mutt \
    bgiarrizzo/neomutt:latest \
    neomutt
```