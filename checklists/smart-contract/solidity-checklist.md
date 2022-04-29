# Solidity Security Checklist
[kompotkot](https://github.com/kompotkot), [Moonstream DAO](https://moonstream.to/)
February 15, 2022

Edited by [YOU](#)

## Description
This checklist is used by Moonstream Dev Team before deploying Solidity Smart Contracts

## Soft checks
- [ ] Code duplication and redundant is minimal
- [ ] Libraries are properly including the specific version(s) that are compatible with project
- [ ] Check the use reasonability of exception in the contract
- [ ] The code compiles with the latest Solidity compiler version
- [ ] There are no compiler warnings, or warnings are documented
- [ ] There are tests with reasonable coverage
- [ ] There are migration scripts
- [ ] The tests are related to the migration scripts and a clear separation is made between the two
- [ ] There is no dead code
- [ ] There is no code in comments
- [ ] There are no getter functions for public variables, or the reason why these getters are in the code is given
- [ ] There are no unnecessary public functions

## Auto-tool checks
- [ ] Run slither. It understands brownie and hardhat config, so there are no needs in additional setup

slither .


- [ ] Run mythril. To analyze contracts which import openzeppelin contracts, you need to clone https://github.com/OpenZeppelin/openzeppelin-contracts.git repository and remap in solc configuration file

{
    "remappings": [ "@openzeppelin-contracts/contracts/=../openzeppelin-contracts/contracts/" ],
    "optimizer": {
        "enabled": true
    }
}

Command to run mythril:

myth analyze contracts/<contract_name>.sol --solc-json solc-remap.json

## Hard checks
- [ ] Access Control & Authorization
	- [ ] Functions access
	- [ ] Variables visibility
- [ ] Safe math
- [ ] Gas Consumption
- [ ] Reentrancy
- [ ] Pseudo-random Number Generator
- [ ] Transaction Order Dependence
- [ ] DoS
- [ ] Call functions security
- [ ] Uninitialized Storage Pointer


# Vulnerabilities Category
Main smart contract vulnerability category that should be evaulated before each deployment

## Access Control & Authorization
Description: Whether the owner has excessive permissions, such as wrong owner or controller setup, modifying balance, variables or other.

## Safe math
Descriptions: Check whether it prevents the integer overflow/underflow in mathematical operation.

SWC: [101](https://swcregistry.io/docs/SWC-101)

## Gas Consumption
Descriptions:
- Check whether the gas consumption exceeds the block gas limitation, or whether it can
be greatly reduced, as example: array of unknown size, etc.
- Check the hardcoded gas amount.
- Check possibilities of insufficient gas use in a sub-call on another contract.

SWC: [128](https://swcregistry.io/docs/SWC-128), [134](https://swcregistry.io/docs/SWC-134), [126](https://swcregistry.io/docs/SWC-126)

## Reentrancy
Description: A malicious contract can call back into the calling contract before the first invocation of the function is finished.

SWC: [107](https://swcregistry.io/docs/SWC-107)

## Pseudo-random Number Generator
Description: Whether the results of random numbers can be predicted.

SWC: [120](https://swcregistry.io/docs/SWC-120)

## Transaction Order Dependence
Description: Whether the final state of the contract depends on the order of the transactions and could be easily read and “race conditioned” by miners, etc.

SWC: [114](https://swcregistry.io/docs/SWC-114)

## DoS
Description: Whether exist DoS attacks in the contract are vulnerable because of unexpected reasons.

## Call functions security
Description: Check whether the usage of functions call/delegatecall have vulnerabilities.

SWC: [112](https://swcregistry.io/docs/SWC-112)

## Uninitialized Storage Pointer
Description: Uninitialized local storage variables can point to other unexpected storage variables in the contract.

SWC: [109](https://swcregistry.io/docs/SWC-109)


## Resource Links
Audit sources
- Hacken audits - https://hacken.io/audits/ 
- CER audits - https://cer.live/audits 
Toolset
- slither github - https://github.com/crytic/slither 
- mythril github - https://github.com/ConsenSys/mythril 
- echidna github - https://github.com/crytic/echidna 
Exploits
- Bridges exploit - https://www.certik.com/resources/blog/technology/cross-chain-bridge-attacks-explained#home 
- Reentrance and transfer() vulnerability - https://consensys.net/diligence/blog/2019/09/stop-using-soliditys-transfer-now/ 
Other
- Hacken whitepaper - https://hacken.ai/content/hackenai_whitepaper_v1.0.pdf 
- Smart Contract Weakness Classification and Test Cases - https://swcregistry.io/ 