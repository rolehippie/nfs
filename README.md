# nfs

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&logoColor=white)](https://github.com/rolehippie/nfs) [![Testing Build](https://github.com/rolehippie/nfs/workflows/testing/badge.svg)](https://github.com/rolehippie/nfs/actions?query=workflow%3Atesting) [![Readme Build](https://github.com/rolehippie/nfs/workflows/readme/badge.svg)](https://github.com/rolehippie/nfs/actions?query=workflow%3Areadme) [![Galaxy Build](https://github.com/rolehippie/nfs/workflows/galaxy/badge.svg)](https://github.com/rolehippie/nfs/actions?query=workflow%3Agalaxy) [![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/nfs)](https://github.com/rolehippie/nfs/blob/master/LICENSE)

Ansible role to install and configure a NFS server.

## Sponsor

Building and improving this Ansible role have been sponsored by my current and previous employers like **[Cloudpunks GmbH](https://cloudpunks.de)** and **[Proact Deutschland GmbH](https://www.proact.eu)**.

## Table of content

- [Default Variables](#default-variables)
  - [nfs_exports](#nfs_exports)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Default Variables

### nfs_exports

List of available exports

#### Default value

```YAML
nfs_exports: []
```

#### Example usage

```YAML
nfs_exports:
  - path: /data/bar
    host: 192.168.0.0/24
    options:
      - rw
      - sync
      - no_subtree_check
  - path: /data/baz
    network: 192.168.0.0/24
```

## Discovered Tags

**_nfs_**


## Dependencies

- None

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)
