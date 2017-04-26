# mastodon-munin-plugins
Some munin plugins to graph Mastodon activity

* local & global toots counts
* open websockets
* confirmed, unconfirmed and remote accounts
* remote instances linked
* toots visibility (smoothed on 24 hours)

## Installation

As root:
```bash
git clone https://github.com/cquest/mastodon-munin-plugins.git
cd mastodon-munin-plugins/
ln -s $PWD/plugins/mastodon_{accounts,follows,statuses,statuses_visibility_local,streams} /etc/munin/plugins/
ln -s $PWD/plugin-conf.d/mastodon /etc/munin/plugin-conf.d/
service munin-node restart
```

## Example

https://mastodon.etalab.gouv.fr/munin/babar/mastodon.babar/index.html#mastodon

