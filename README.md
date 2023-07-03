# ansible-docker-migrid
A collection of tools for automating docker-migrid deployment on a physical or virtual machibe with ansible

## Prerequisites

* Install dependencies: `ansible-galaxy install -r requirements.yml`

## Installation

This repo can be used as a collection. Use the following command to install it

```
ansible-galaxy collection install https://github.com/ucphhpc/ansible-docker-migrid.git
```

or add it to your `requirements.yml` like this:

```
collections:
  - name: https://github.com/ucphhpc/ansible-docker-migrid.git
    type: git
    version: main
```

## Usage

Afterwards the roles can be used like this:

```
  roles:
    - ucphhpc.docker_migrid.setup_vars
    - ucphhpc.docker_migrid.migrid_pre_check
    ...
```
