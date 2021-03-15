---
title: How to Run a Node
lang: en-US
tags:
    - node
    - verifier
    - high-level
---

# {{ $frontmatter.title }}


## Running a node locally

Spin up a Layer 1 (Ethereum) node on port 9545 and a Layer 2 (Optimistic Ethereum) node on port 8545:

```
git clone git@github.com:ethereum-optimism/optimism-integration.git --recurse-submodules
cd optimism-integration
docker-compose pull
make up
```

* Change configuration in [`docker-compose.env.yml`](https://github.com/ethereum-optimism/optimism-integration/blob/master/docker-compose.env.yml).
* **Default chain ID is 420**.
* Transactions are free in dev mode, no need to give yourself a balance.
