# neovim

neovim container

## Build

```bash
docker build -t bgiarrizzo/neovim:latest -f Containerfile .
```

## Run

```bash
docker run -it --rm --name $(whoami)-neovim \
    -v ${HOME}/.config/neovim:/home/user/.config/neovim \
    -v ${HOME}/.local/share/neovim:/home/user/.local/share/neovim \
    -v ${HOME}/.neovim:/home/user/.neovim \
    -v ${HOME}/.cache/neovim:/home/user/.cache/neovim \
    bgiarrizzo/neovim:latest \
    nvim 
```