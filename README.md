# blockmaze-mainnet-script

This repository provides ubuntu 22.04 and 24.04 script for running a node on blockmaze mainnet:

System Requirements:

- Operating System: Ubuntu 22.04 or 24.04
- Memory: At least 16GB RAM
- Storage: Minimum 20GB available disk space
- Network: Stable internet connection
- CPU: 4core

Clone this repo using:
git clone '<https://github.com/NodeNavigator/blockmaze-mainnet-script.git>'

Setup the node:
open a terminal window and run the following command:

```bash
./install-go.sh
```

after that
```bash
source ~/.profile
source ~/.bashrc
```


Start a Node from the Genesis Block
```bash
./blockmaze_ubuntu_node.sh
```


Start a Node Using State Sync
Sync the node quickly with the latest available blockchain state.
```bash
./node_state_sync.sh
```



once it finishes, start the node service with the following command:

```bash
sudo systemctl start blockmazechain.service
```

check the node logs with the following command:

```bash
journalctl -u blockmazechain.service -f
```
