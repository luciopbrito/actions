# Actions

This repository is inspired by [@devopselvis](https://github.com/devopselvis/).

I will save actions that I use frequently in my repositories.

## Table of Contents

1. SSH related
    - [Save SSH Key Actions](#save-ssh-key)
    - [Clean SSH Key Actions](#clean-up)

### Save SSH Key

This action saves an SSH key in the `/tmp/id_rsa` path of the current runner and tests the connection before it.

#### How to Use Save SSH Key Action

It is necessary to declare these secrets below:

- `SSH_PRIVATE_KEY`
- `SSH_HOST`
- `SSH_PORT`
- `SSH_USERNAME`

##### Parameters

- ssh-key-path – Destination of SSH Key. As default `/tmp/id_rsa`

### Clean Up

This action cleans the SSH key context of the current runner

#### How to Use Clean Up Action

There is an optional parameter to specify the locale of the SSH Key. It is the same value of ssh-key-path from [save ssh key](#save-ssh-key).
