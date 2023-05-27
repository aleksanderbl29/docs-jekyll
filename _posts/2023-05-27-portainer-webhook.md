---
title: Deploying a docker stack in portainer with webhooks for automatic updates
date: 2023-05-27 09:00:00 +0200
categories: [Homelab, Portainer]
tags: [homelab, learning, portainer, webhook]     # TAG names should always be lowercase
mermaid: true
img_path: /media/portainer-docker-compose-stack/
---
In this project i wanted to deploy a docker-compose file hosted on github and prepare a webhook that i can call to redeploy the docker-compose file.
## What you'll need
* Portainer BE
* Docker environment
* Github repo with docker-compose file

## Deploying the stack
1. You should go to your environment.


2. We will be working in "stacks" today.

![Light mode only](stacks-light.png){: .shadow .light}
![Dark mode only](stacks-dark.png){: .shadow .dark}

3. Choose "add stack" in the top right corner.
4. Then choose "Repository"

![Light mode only](git-add-stack-light.png){: .shadow .light}
![Dark mode only](git-add-stack-dark.png){: .shadow .dark}

5. Then insert the url of your repository

![Light mode only](url-light.png){: .shadow .light}
![Dark mode only](url-dark.png){: .shadow .dark}

6. Then insert the path of your docker-compose file from github

![Light mode only](path-light.png){: .shadow .light}
![Dark mode only](path-dark.png){: .shadow .dark}

7. Then enable automatic updates and choose "webhook"

![Light mode only](auto-light.png){: .shadow .light}
![Dark mode only](auto-dark.png){: .shadow .dark}