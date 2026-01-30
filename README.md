# CacheGPT
CacheGPT : Un cache qui apprend en continue et s'auto-optimise en local ou à proximité (MANET). Cela permet de retrouver une réponse localement si la question à déjà été posé sans réitérer. L'objectif est uniquement d'optimiser ce qui existe déjà. Le modèle ne fera pas une grande taille étant donnée que l'objectif est de fournir un accès rapide.

# Architecture

Model --> MCP + Prompting --> Cache + Response : 
- --> Answering
- --> Save in Cache for later

Whether there's no Internet network, the DNS server can switch to CacheGPT to get some Informations (Data, cache state, etc...) quickly.

# Technology to use : Python and caching

In python, we will implement a tree : 
- Each leaf must implement a caching level.
- Using decorators : @decorator for declaring caching.
- Each node has its own cache level and logical storage to benefit cache speed.

Ins this moment, i think i could change to Java Implementation to benefit already implemented code by others devs.
