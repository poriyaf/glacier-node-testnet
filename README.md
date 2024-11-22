# Glacier Node Testnet

| **Hardware** | **Minimum Requirement** | **Recomendation Requirement** |
|--------------|-------------------------|-------------------------------|
| **CPU**      | 1 Cores                 | 2+ Cores                      |
| **RAM**      | 2 GB                    | 4+ GB                         |
| **Internet** | 4 Mbit/s                | 8+ Mbit/s                     |

# Installation

## Manual

```
source <(curl -s https://raw.githubusercontent.com/ryzwan29/glacier-node-testnet/main/quick-installation.sh)
```
```
nano config.yaml
```
Replace the ```PrivateKey``` in the ```config.yaml``` with your privatekey.
After replacing the KN privit, save it with the following command and exit with CTRL+X+Y+ENTER
Using the links below, first get faucet bnb and then convert it with opbnb.
### Run the Node
```
screen -R glacier
```
```
./verifier_linux_amd64
```
Wait for it to run, then close the screen with CTRL+A+D

## Docker

```
docker run -d -e PRIVATE_KEY=$YOUR_PRIVATE_KEY --name glacier-verifier docker.io/glaciernetwork/glacier-verifier:v0.0.1
```
Replace the ```PRIVATE_KEY``` with your privatekey.

# Useful Resource
- [Register Here](https://www.glacier.io/points/?inviter=0x060CCc6a55679b71154b0aea8FACAB3894e5b483)
- [Bridge BNB Testnet to opBNB Testnet](https://opbnb-testnet-bridge.bnbchain.org/deposit)
- [Faucet BNB](https://faucet.quicknode.com/binance-smart-chain/bnb-testnet)
- [Faucet BNB](https://faucet.chainstack.com/bnb-testnet-faucet)
- [Faucet BNB](https://thirdweb.com/opbnb-testnet)
- [Check Wallet Status](https://testnet.nodes.glacier.io/status) (After Run the Node)
