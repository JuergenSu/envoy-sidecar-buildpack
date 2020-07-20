# envoy-sidecar-buildpack

This envoy sidecar buildpack does start an envoy proxy on port `61011` using the application instance certificate and key. It allows easy configuration for TLS with container to container networking.

Usage:

`cf push -b https://github.com/vchrisb/envoy-sidecar-buildpack -b java_buildpack_offline`

`cf add-network-policy source destination --protocol tcp --port 61011`
