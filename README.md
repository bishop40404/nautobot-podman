# Nautobot in Podman

Nautobot-podman is a deployment of [Nautobot](https://github.com/nautobot/nautobot) in rootless podman with a nginx frontend.

## How to use

This repo is a build guide. Start at 1 and read through, executing commands. It might work if you download and directly execute the .txt files, but I have not tried. I separate the bull, create, and start commands to better support isolated deployments and offer better control.

**1. System Setup** - Run system pre-requisites. Create your cert, edit config files, put them in the right place

**2. Podman Pull Commands** - Pull or build containers

**3. Podman Create Commands** - Create the containers

**4. Podman Start Commands** - Start all the containers and create your superuser
