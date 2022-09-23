! Note: This is a template/example, this repository should be not exactly copied into your production flow.

# Automated Infrastructure

:construction: (WIP) automated infrastructure using ansible, docker, dockerswarm, terraform

This idea came up when I had so many software to deploy. And... Most of the time, they are practically the same.
- create an infrastructure
  - Add a server for loadbalancing, N Worker nodes, N database node, 1 monitoring server, N extra servers for god-only-knows-what-you-will-do-with-it.
- tagging each servers
  - most of the time you want to give them some kind of name, or tagging. So whenever you talk to your team. You don't talk about numbers and weird words. Like "server-ng-10-a died OMG!!" But be meaningful; i.e giving a name to servers. Ex. giving nordic/greek/egyptians/roman (or french?) names to your servers.
  - Serve yourself with any mythology you want [here](https://en.wikipedia.org/wiki/List_of_mythologies).
- configure the servers
  - you need to install some prerequisites on your servers, doing `apt install something-something` or placing configuration files manually into servers are a bit tiring... imagine you have an infrastructure of 10 nodes...or...even more. ([RIP](https://youtu.be/gDLnAjvcJgA))
- managing access
  - everyone should not be able to ssh into your servers right?
- managing firewall
  - having a firewall is actually [noice](https://www.youtube.com/watch?v=h3uBr0CCm58).
- deploy your code in an orchestrated manner
  - I use docker swarm for that, it is pretty good.
- monitoring your servers
  - Knowing what is going on on your servers
    - using Grafana, Loki, Prometheus (with exporters)


# Requirements
For this automated infrastructure you will need:
- Docker
- Access to a provider: AWS/Azure and other supported by Terraform.
- Ansible


