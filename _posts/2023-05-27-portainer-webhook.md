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
You should go to your environment. We will be working in "stacks" today.

![Light mode only](stacks-light.png){: .shadow .light}
![Dark mode only](stacks-dark.png){: .shadow .dark}

Choose "add stack" in the top right corner. Then choose "Repository"

![Light mode only](git-add-stack-light.png){: .shadow .light}
![Dark mode only](git-add-stack-dark.png){: .shadow .dark}

Then insert the url of your repository

![Light mode only](url-light.png){: .shadow .light}
![Dark mode only](url-dark.png){: .shadow .dark}

Then insert the path of your docker-compose file from github

![Light mode only](path-light.png){: .shadow .light}
![Dark mode only](path-dark.png){: .shadow .dark}

Then enable automatic updates and choose "webhook"

![Light mode only](auto-light.png){: .shadow .light}
![Dark mode only](auto-dark.png){: .shadow .dark}

When you have copied your webhook url you can safely click deploy

![Light mode only](deploy-light.png){: .shadow .light}
![Dark mode only](deploy-dark.png){: .shadow .dark}

## That's it!
You now have a docker-compose file that redeploys itself when the webhook url is called.