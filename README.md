# ZeroTier proof-of-concept

[![Import](https://cdn.infobeamer.com/s/img/import.png)](https://info-beamer.com/use?url=https://github.com/info-beamer/package-zerotier)

This package adds [ZeroTier](https://zerotier.com/) support to any
of your existing setups. Just add this package
as a child package, configure a network and
then go to your ZeroTier management dashboard
to authorize your devices once they automatically
joined.

The ZeroTier daemon also accepts adding external
default routes, so you can add an "exit node"
as described [here](https://zerotier.atlassian.net/wiki/spaces/SD/pages/7110693/Overriding+Default+Route+Full+Tunnel+Mode)
to route all traffic through your own router.

Note that the persistent websocket connection to
the info-beamer hosted backend will have to timeout
when you overwrite the default route. So your
devices might appear offline for a minute or two.

info-beamer P2P also works and should be able to
reach all nodes in your network.
