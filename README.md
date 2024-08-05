# thegraph-project

This project is a simple example of how to use thegraph to index data from a smart contract and query it using a subgraph.

## Getting Started

### Subgraph URL: [https://api.studio.thegraph.com/query/85765/foundation-nft/v0.0.1](https://api.studio.thegraph.com/query/85765/foundation-nft/v0.0.1)

### Example Query

```graphql
query {
  transfers(first: 100, orderBy: timestamp, orderDirection: desc) {
    id
    from {
      id
    }
    to {
      id
    }
    tokenId
    transactionHash
    timestamp
  }
}
```
