# hardhat-template

No more dependencies using [vscode](https://code.visualstudio.com/) and [docker](https://www.docker.com/)

⛓️🤍🐋

## you will need

👉 [Infura](https://www.infura.io/) API key

👉 [MetaMask](https://metamask.io/) address into sepolia test net

## step by step

1. Install [docker](https://docs.docker.com/engine/install/) within the preferred operating system.
2. Open vscode and install [remote development plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack) typing `Ctrl + P` and pasting `ext install ms-vscode-remote.vscode-remote-extensionpack`.
3. Clone this repository:

```bash
git clone git@github.com:hardenerdev/hardhat-template.git -b blockchain-malaga-workshop
```
4. Create `.env` file and set your credentils:

```bash
cd hardhat-template
cp .env.local .env
```
5. Open directory in container using `Ctrl + P`, choose `Dev Containers: Open Folder in Container...` and open repository folder.
6. Open a terminal inside vscode (``Ctrl + Shift + ` ``) and execute hardhat commands

```bash
npx hardhat compile
npx hardhat test
REPORT_GAS=true npx hardhat test
npx hardhat node
npx hardhat run scripts/deploy.js
npx hardhat run scripts/deploy.js --network localhost
```
7. Deploy to sepolia test net:

```bash
npx hardhat run scripts/deploy.js --network localhost
```

⛓️🤍🐋
