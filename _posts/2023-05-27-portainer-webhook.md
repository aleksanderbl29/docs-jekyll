---
title: Deploying a docker stack in portainer with webhooks for automatic updates
date: 2023-05-27 09:00:00 +0200
categories: [Homelab, Portainer]
tags: [homelab, learning, portainer, webhook]     # TAG names should always be lowercase
mermaid: true
img_path: aleksanderbl29.github.io/media/portainer-docker-compose-stack/
---
In this project i wanted to deploy a docker-compose file hosted on github and prepare a webhook that i can call to redeploy the docker-compose file.
## What you'll need
* Portainer BE
* Docker environment
* Github repo with docker-compose file
## Deploying the stack
You should go to your environment.
We will be working in "stacks" today.
![Light mode only](stacks-light.png){: .normal .shadow .light}
![Dark mode only](stacks-dark.png){: .normal .shadow .dark}