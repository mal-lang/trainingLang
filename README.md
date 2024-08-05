# trainingLang
A simple MAL language used to create simple models and attack graphs for machine learning agents training.

# How to compile trainingLang

1. Download and install malc: `git@github.com:mal-lang/trainingLang.git`

2. Clone this repository

3. Compile trainingLang: `malc trainingLang/src/main/mal/trainingLang.mal`

`malc` will generate a .mar-archive that can be used by MAL Toolbox to generate AttackGraphs.
TODO: Link to docs on how to do that.

# trainingLang
The goal of trainingLang is to be simple but still feature several types of assets and associations.
We want to keep number of attack steps low to result in smaller attack graphs.

# Assets

## Host

Represents a host in a network and can have users and data connected to it.

### Associations 

Host is part of three associations:
- **NetworkHostAccess**: Network (networks) -> Host (hosts)
- **HostUsers**: User (users) -> Host (hosts)
- **HostData**: Host (hosts) -> Data (data)

Note: List above on format `<Asset type> (<field name>) -> <Asset type> (<field name>)`

## Data

Represents data that can be on a host,

Host is part of one association:
- **HostData**: Host (hosts) -> Data (data)


## Network

Represents a network that hosts and networks can have access to.

Network is part of two associations:
- **NetworkHostAccess**: Network (networks) -> Host (hosts)
- **NetworkToNetworkAccess**:  Network (network) -> Network (networks)


## User

Represents a user that has access to hosts.

Host is part of one association:
- **HostUsers**: User (users) -> Host (hosts)
