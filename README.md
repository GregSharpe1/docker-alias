# Docker Aliases

I use aliases for various things, [here](https://github.com/GregSharpe1/alias). This repository is setup for using Docker containers as various applications within my local machine. 

## Why?

For example, I don't want to install [Terraform](terraform.io/) because I often find I need to use various versions across different project, so within (terraform)[./terraform], I have defined [versions](./versions) file.

## How to use?

1. Clone the repository into `~/.docker/docker-alias` directory.

2. Place the following with `~/.$SHELLrc` file.

```
# Source docker function calls
for f in $HOME/.docker/docker-alias/*.alias; do source $f; done
# Source the versions
source $HOME/.docker/docker-alias/versions
```

## Using the following

While I will try and keep this repository updated I may not be able to assure the usability of each "alias" / "container". There's my warning, don't point at me when shit breaks.