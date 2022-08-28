# NFT Minting App for Solana

## Setup

Use the package manager npm to install required packages.

* First install sugar machine as binary to your computer
```bash
bash <(curl -sSf https://sugar.metaplex.com/install.sh)
```
required configuration should completed by following this tutorial 

[Setup Tutorial This Link](https://docs.metaplex.com/developer-tools/sugar/tutorials/my-first-candy-machine)



## Usage
* First Prepare your assets as ordered way 
* You should prepare your assets and asset metada from template below 
* !!! This metadata for images 
````
{
  "name": "Number #0001",
  "symbol": "NB",
  "description": "Collection of 10 numbers on the blockchain. This is the number 1/10.",
  "image": "0.png",
  "attributes": [
    {
      "trait_type": "Number",
      "value": "0"
    }
  ],
  "properties": {
    "files": [
      {
        "uri": "0.png",
        "type": "image/png"
      }
    ]
  }
}
````
* Upload your metada and assets to [Pinata](https://www.pinata.cloud/)  Cloud for IPFS 
* When your assets ready to minting and sugar machine configuration is completed then Run commands below
```
sugar launch // to launch sugar machine 
sugar upload // upload assets and check them is valid ot not valid
```
```
sugar deploy // deploy your machine to solana
```

```
sugar verify // after this command candy machine will give you to your machine url 
```

## Sugar Machine UI for minting assets

We will use metaplex open source UI for this project 
[Candy Machine UI](https://github.com/metaplex-foundation/candy-machine-ui) dowload and install packages required

## Example Commands File for Sugar Machine
[commands file ](https://gist.github.com/doingthisalright/9e3b049edaf8415a204194fd8d0e2438)