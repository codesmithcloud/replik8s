![GitHub branch status](https://img.shields.io/github/checks-status/codesmithcloud/replik8s/main)
![GitHub License](https://img.shields.io/github/license/codesmithcloud/replik8s)
![GitHub Release](https://img.shields.io/github/v/release/codesmithcloud/replik8s)


# replik8s

Kubernetes controller for synchronising Kubernetes resources across namespaces.

replik8s supports **all Kubernetes resources - including Custom Resources**.

If it has an `apiVersion` and a `kind`, replik8s can replicate it!

Tested with:

* ConfigMap
* Secret
* Role
* NetworkPolicy
* Service
* Deployment
* Ingress
* Gateway
* Certificate
* CertificateRequest
* CertificateSigningRequest
* HTTPRoute

### [Quick Start](https://replik8s.codesmith.cloud) | [Full documentation](https://replik8s.codesmith.cloud)

## Credits

The full documentation for the replik8s project - stored in the [./docs](./docs) directory - has been built using [Docus](https://docus.dev),
which is an open source project that can be used to write documentation that looks absolutely fantastic.

It has made writing the documentation for this project far less taxing than it would have been otherwise. Kudos to everybody involved in that project, and the giants whose shoulders Docus stands upon.
