# newsboat

newsboat container

## Build

```bash
docker build -t bgiarrizzo/newsboat:latest -f Containerfile .
```

## Run

```bash
docker run -it --rm --name $(whoami)-newsboat \
    -v ${HOME}/.config/newsboat:/home/user/.config/newsboat \
    -v ${HOME}/.newsboat:/home/user/.newsboat \
    -v ${HOME}/.cache/newsboat:/home/user/.cache/newsboat \
    bgiarrizzo/newsboat:latest \
    newsboat -r
```