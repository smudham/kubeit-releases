# KubeIt — Releases

Public downloads for **KubeIt**, a native macOS Kubernetes IDE built with SwiftUI + Rust.

## Download

Grab the latest **KubeIt.zip** from the [latest release](https://github.com/smudham/kubeit-releases/releases/latest):

1. Unzip and move **KubeIt.app** to `/Applications`.

KubeIt updates itself — once installed, new versions arrive via **KubeIt → Check for Updates…**

## Found a bug?

[**Open an issue**](https://github.com/smudham/kubeit-releases/issues/new) and it'll get looked at.

To make it fixable first time, include:

- **KubeIt version** — *KubeIt → About KubeIt*
- **macOS version**
- **Your shell** — run `echo $SHELL` in Terminal
- **Cluster type** — GKE, EKS, AKS, OCI, kind/minikube, on-prem…
- **The full error text**, if there is one

If it's a **connection or authentication** failure, also paste the output of:

```sh
echo $SHELL
command -v gke-gcloud-auth-plugin   # GKE
command -v aws                      # EKS
command -v oci                      # OCI
```

Those two — your shell and whether the auth helper is on your `PATH` — are what most
connection failures come down to, and they're the hardest things to guess from the error
message alone.
