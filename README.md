# pra-client

A client workload in the `e5-client` cluster that calls `hello` in the
`e5-server` cluster at a steady rate. It dials `api.e5.internal:8443`; how
that name reaches the server is the platform's business (see `pra-infra`).

`deploy/client.yaml` holds the Deployment and its ConfigMap. The call rate
is `CALL_INTERVAL` seconds between calls.
