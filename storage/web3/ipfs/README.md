**IPFS**

1. When you add a file to IPFS it is split into cryptographically hashed smaller chunks and then given a unique fingerprint called a content identifier (CID).

2. When a node looks up for a file, it ask the peer nodes for the content referenced by the file's CID. When a node views or downloads a file, it caches a copy and become another provider until the cache is cleared.

3. When you add a new version of your file to IPFS it will get a new CID since the cryptographic hash is different. This means that any changes to a file will not overwrite the original and common chunks across files can be reused in order to minimize storage costs.
IPFS offers a decentralized naming system so you don't need to remember a long string of CIDs. IPFS can find the latest version of your file using the IPNS decentralized naming system and you can use DNSLink to map CIDs to human-readable DNS names.
