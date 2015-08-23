# elastizabbix
Down and dirty elastic / elasticsearch monitoring plugin for zabbix

## Features:

- Stats cache to avoid saturating nodes with monitoring requests
- Node and index low-level (auto) discovery
- JSON-like dot notation item syntax for easy customization
- Can monitor anything elastic exposes in the stats API

## Installation

This only needs to be setup on one of the elasticsearch nodes

#### Zabbix Agent

- Copy elastizabbix to agent scripts folder
- Copy elastizabbix.conf to conf.d or add UserParameter to your agent config

#### Zabbix Frontend

- Import the XML template
- Add node to the newly imported template
