# Overall status
GA

# Supported CSI spec versions
1.0-1.4

# Minimum Kubernetes version
1.17

# Recommended Kubernetes version
1.21: For capacity reporting beta\
1.18: For cloning GA

# Container
`docker pull k8s.gcr.io/sig-storage/csi-provisioner:v2.2.0`

# Deprecations
All external-provisioner versions < 1.4.0 are deprecated and will stop functioning in Kubernetes v1.20. See #323 and k/k#80978 for more details. Upgrade your external-provisioner to v1.4+ before Kubernetes v1.20.

# Feature status
| Feature | Status | Default | Description | Provisioner Feature Gate Required |
|---|---|---|---|---|
| Snapshots | Beta | On | [Snapshots and Restore]. | No |
| CSIMigration | Beta | On | [Migrating in-tree volume plugins to CSI]. | No |
| CSIStorageCapacity | Beta | On | Publish [capacity information] for the Kubernetes scheduler. | No |

[Snapshots and Restore]: https://kubernetes-csi.github.io/docs/snapshot-restore-feature.html
[Migrating in-tree volume plugins to CSI]: https://kubernetes.io/docs/concepts/storage/volumes/#csi-migration
[capacity information]: https://kubernetes.io/docs/concepts/storage/volumes/#storage-capacity

# Full Changelog
https://github.com/kubernetes-csi/external-provisioner/blob/release-2.2/CHANGELOG/CHANGELOG-2.2.md
