# IPFS Cluster - Collaborative Clusters

*Collaborative clusters* are public IPFS Clusters that anyone can join to help replicating and re-distributing content on the IPFS network.

* [List of clusters](#list-of-clusters)
* [How to run a follower peer](#instructions)
* [Helping the project](#helping-the-project)

---

## List of Clusters

| | [Filecoin Params](https://filecoin.io) |
| - | - |
| **Description** | The Filecoin cluster holds filecoin proofs and filecoin-related binaries. |
| ***Init&Run*** | `ipfs-cluster-follow filecoin run --init filecoin.collab.ipfscluster.io` |
| **Size** | 100GB (expected to grow over time to 500GB) |
| **Cluster version** | 0.12.0 |
| **Hosted by** | Protocol Labs |

---

| | [Project Gutenberg (Spanish)](https://gutenberg.org) |
| - | - |
| **Description** | Spanish eBooks from Project Gutenberg, in HTML format. |
| ***Init&Run*** | `ipfs-cluster-follow gutenberg_es run --init gutenberg-es.collab.ipfscluster.io` |
| **Size** | 1GB |
| **Cluster version** | 0.12.0 |
| **Hosted by** | Protocol Labs |
| **Tooling** | [gutenberg-to-ipfs repository](https://github.com/ipfs-shipyard/gutenberg-to-ipfs) |

---

| | IPFS Websites |
| - | - |
| **Description** | A collection of IPFS related websites (ipfs.io, libp2p.io, docs.ipfs.io...) |
| ***Init&Run*** | `ipfs-cluster-follow ipfs-websites run --init ipfs-websites.collab.ipfscluster.io` |
| **Size** | 600MB |
| **Cluster version** | 0.12.0 |
| **Hosted by** | Protocol Labs |
| **Tooling** | [pin-websites.sh](https://github.com/ipfs-cluster/archive-tools/blob/master/ipfs-websites/pin-websites.sh) |

---


## Instructions

You can join a collaborative cluster by running a "follower" peer (a peer without write access to the Cluster's pinset). In order to run a follower peer:

* Start your [go-ipfs](https://github.com/ipfs/go-ipfs#install) daemon online.
* Download the [ipfs-cluster-follow](https://dist.ipfs.io/#ipfs-cluster-follow) application.
* Execute the *Init&Run* command from the Cluster descriptions above, after starting your IPFS daemon. This will initialize and run the peer, which will pin archive items to your IPFS daemon.
* To check what is being pinned by this cluster, run `ipfs-cluster-follow <clusterName> list`

Note that `ipfs-cluster-follow` **will try to pin the full archive, so you will need at least as much space available in your node as the *Size* requirement indicates** for each archive.

Follow as many collaborative clusters as you want, the different follower peers will run in parallel!

You can obtain more help about `ipfs-cluster-follow` usage [here](https://cluster.ipfs.io/documentation/reference/follow/).


---

## Helping the project

Help us distribute and backup important data on the IPFS network. You can help us by:

* Proposing new, interesting archives that we can distribute through new Clusters.
* Hosting new collaborative clusters yourself (see documentation in the [IPFS Cluster website](https://cluster.ipfs.io/documentation/collaborative/)
* Improving [this website](https://github.com/ipfs-cluster/collab.ipfscluster.io)
* Reporting issues that you encounter, asking questions and distributing the word: [https://cluster.ipfs.io/support/](https://cluster.ipfs.io/support/)
