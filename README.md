# Actions

This repository is inspired by [@devopselvis](https://github.com/devopselvis/).

I will save actions that I use frequently in my repositories.

## Table of Contents

- SSH

  - [Save SSH Key Actions](#save-ssh-key-action)

  - [Clean SSH Key Actions](#clean-up-ssh-action)

- .NET

  - [Build version](#net-build-version)

### Save SSH Key Action

This action saves an SSH key in the `/tmp/id_rsa` path of the current runner and tests the connection before it.

#### How to Use Save SSH Key Action

It is necessary to declare these secrets below:

- `SSH_PRIVATE_KEY`

- `SSH_HOST`

- `SSH_PORT`

- `SSH_USERNAME`

##### Save SSH Key Action — Inputs

- `ssh-key-path` — Destination of SSH Key. As default `/tmp/id_rsa`

##### Save SSH Key Action — Outputs

- `ssh-key-path` — Destination of SSH Key. As default `/tmp/id_rsa`

### Clean Up SSH Action

This action cleans the SSH key context of the current runner

#### How to Use Clean Up Action

There is an optional parameter to specify the locale of the SSH Key. It is the same value of ssh-key-path from [save ssh key](#save-ssh-key-action).

##### Clean Up SSH Action — Inputs

- `ssh-key-path` — Destination of SSH Key. As default `/tmp/id_rsa`

### .NET build version

This action builds a version of the current context and uploads an artifact.

#### How to use .NET build version

It is necessary to set up the path that contains the solution file, and the `.tool-versions` file needs to be defined.

#### .NET build version — Outputs

- `version_built` — version that will be build.
