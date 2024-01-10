# inst-k3s
This repository contain two bash script used for install and configure an simple k3s cluster with longhorn and metallb.

# inst-k3s-master
This simple script, actually can be runned only on debian or ubuntu enviroment, install all required package for run an k3s master node with longhorn and metallb.

- upgrade your system
- install curl
- install docker by docker public script
- install open-iscsid anf nfs-common
- install k3s master without servicelb
- deploy longhorn and metallb l2
- configure filesystem and replica in default storageclass

This script support some options for specify storageclass configuration. \
For more info run:

```bash
./inst-k3s-master -h
```

or

```bash
./inst-k3s-master --help
```
# inst-k3s-client
This simple script, actually can be runned only on debian or ubuntu enviroment, install all required package for run an k3s agent node with longhorn and metallb.

- upgrade your system
- install curl
- install docker by docker public script
- install open-iscsid anf nfs-common
- install k3s client

This script require some options for set master ip and node token. \
For more info run:

```bash
./inst-k3s-client -h
```

or

```bash
./inst-k3s-client --help
```
