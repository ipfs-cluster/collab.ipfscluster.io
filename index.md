## Collaborative Clusters

*Collaborative clusters* are public IPFS Clusters that anyone can join to help replicating and re-distributing content on the IPFS network.

* [List of clusters](#list-of-clusters)
* [How to run a follower peer](#instructions)
* [Helping the project](#helping-the-project)

### List of Clusters

---

| | Filecoin cluster |
| - | - |
| **Description** | The Filecoin cluster holds filecoin proofs and filecoin-related binaries. |
| ***Init&Run*** | ```ipfs-cluster-follow filecoin --init filecoin.collab.ipfscluster.io run``` |
| **Size** | 600GB |
| **Version** | 0.12.0 |
| **Hosted by** | Protocol Labs |


### Instructions

When joining a collaborative cluster you become a "follower". In order to run a follower peer:

* To keep your [go-ipfs](https://github.com/ipfs/go-ipfs#install) daemon online.
* To download the [ipfs-cluster-follow](https://dist.ipfs.io/#ipfs-cluster-follow) application.
* Execute the *Init&Run* command from the Cluster description above after starting your IPFS daemon. This will:
  * Generate a new peer identity when no identity exists before
  * Run a follower peer by fetching a configuration template specific for that Cluster
  * Sync and instruct the IPFS daemon what to pin

You can obtain more help about `ipfs-cluster-follow` usage [here](https://github.com/ipfs/ipfs-cluster/blob/master/cmd/ipfs-cluster-follow/dist/README.md).

You can follow as many collaborative clusters as you want. The different follower peers will run in parallel!

### Helping the project

Help us distribute and backup important data on the IPFS network. You can help us by:

* Proposing new, interesting archives that we can distribute through new Clusters.
* Hosting new collaborative clusters yourself (see documentation in the [IPFS Cluster website](https://cluster.ipfs.io)
* Improving [this website](https://github.com/ipfs-cluster/collab.ipfscluster.io)
* Reporting issues that you encounter, asking questions and distributing the word: https://cluster.ipfs.io/support/
