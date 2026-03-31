# Home Assistant Custom Add-on: Portainer

![Warning][warning_stripe]

> This is a **fork** of the deprecated [community add-on][community_addon]!
>
> This makes it available again.

![Warning][warning_stripe]

Portainer is an open-source lightweight management UI which allows you to
easily manage a Docker host(s) or Docker swarm clusters.

It has never been so easy to manage Docker. Portainer provides a detailed
overview of Docker and allows you to manage containers, images, networks and
volumes.

## Installation

To install this add-on, you'll first need to go to your profile and turn on
"Advanced Mode", once that is done go back to Home Assistant add-ons and search
for "Portainer" and install it as you would any other add-on.

To be able to use this add-on, you'll need to disable protection mode on this
add-on. Without it, the add-on is unable to access Docker.

1. In Home Assistant, go to **Settings** -> **Apps** -> **Install app**.
1. In the **...** menu at the top right corner click **Repositories**, add
   `https://github.com/lmagyar/homeassistant-addon-portainer` as repository.
1. Find the "Portainer" add-on and click it. If it doesn't show up, wait until
   HA refreshes the information about the add-on, or click **Check for updates**
   in the **...** menu at the top right corner.
1. Click on the "INSTALL" button.

## How to use

1. Under the Info tab set the "Protection mode" switch to off.
1. Start the add-on.
1. Check the add-on log output to see the result.

## Add-on Configuration

```yaml
agent_secret: password
```

### Option: `agent_secret`

An option to set a shared agent secret. Must also be set in the remote agent
as an Environment variable.

## Support

Got questions?

You have several options to get them answered:

- The [Home Assistant Discord chat server][discord].
- The Home Assistant [Community Forum][forum].
- Join the [Reddit subreddit][reddit] in [/r/homeassistant][reddit]

You could also [open an issue here][issue] on GitHub.

[discord]: https://discord.gg/c5DvZ4e
[forum]: https://community.home-assistant.io/t/home-assistant-community-add-on-portainer/68836
[issue]: https://github.com/lmagyar/homeassistant-addon-portainer/issues
[reddit]: https://reddit.com/r/homeassistant
[warning_stripe]: https://github.com/lmagyar/homeassistant-addon-portainer/raw/main/images/warning_stripe_wide.png
[community_addon]: https://github.com/hassio-addons/addon-portainer
