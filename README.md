# docker-secure-keys-generator
Simple commands that help to generate TSK keys for docker server and docker api client to secure docker API connection

Wery hand to setup docker engines in shipyard

## Usage:

1. `mk-ca` # Will ask you few questions and create `ca` foilder with `ca.pem` and `ca-key.pem`

2. `mk-server-key domain [ip]` # Will ask you few questions and create `domain-key.pem` and `domain-cert.pem` signed with `ca/ca-key.pem`

If ip is not privided it will be resolved automaticaly

3. `mk-client-key` # Will create `client-key.pem` and `client-cert.pem` signed with `ca/ca-key.pem`.
