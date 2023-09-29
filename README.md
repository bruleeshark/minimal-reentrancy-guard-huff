# minimal ReentrancyGuard.huff

How to Use:
## Integration:
Integrate this ReentrancyGuard.huff contract into your project by including it in your project's contracts directory.

Then, import this huff contract in your other .huff contracts and "bracket" the function you wish to guard from reentrancy, with the reentrancy guard template functions found in ReentrancyGuard.huff.

Alternatively, use this as a Huff language learning tool by comparing and contrasting with the (superior, and clearly Error Coded) solmate-esque implementation found at this link; https://github.com/huff-language/huffmate/blob/main/src/utils/ReentrancyGuard.huff 

## Modification:
Modify the :function_call label to include the actual function code that you want to protect against reentrancy attacks.

## Compilation:
Compile the ReentrancyGuard.huff contract using a Huff compiler to generate the corresponding EVM bytecode.

## Deployment:
Deploy the compiled bytecode to the Ethereum network using a deployment script or a deployment tool.

## Interaction:
Interact with the deployed contract by sending transactions to it. The ReentrancyGuard.huff contract will ensure that the function is not reentrant by checking and modifying the lock state in storage.

## @dev Note:
Ensure that the storage slot 0 is not used by other parts of your contract, as it is used by the ReentrancyGuard.huff contract to store the lock state.

Test contract implementation thoroughly to ensure that it works as expected and provides  necessary protection.

## Disclaimer

_These smart contracts are being provided as is. No guarantee, representation or warranty is being made, express or implied, as to the safety or correctness of the user interface or the smart contracts. They have not been audited and as such there can be no assurance they 

# devtooligan -template
[![ci](https://github.com/devtooligan/devtooligan-template/actions/workflows/ci.yml/badge.svg)](https://github.com/devtooligan/devtooligan-template/actions/workflows/ci.yml) ![solidity](https://img.shields.io/badge/Solidity-8.15.0-blue) ![huff](https://img.shields.io/badge/Huff-0.2.0-blue) ![Foundry](https://img.shields.io/badge/Foundry-blue) ![license](https://img.shields.io/github/license/devtooligan/devtooligan-template) ![license](https://img.shields.io/twitter/follow/devtooligan?label=Follow)

Versatile Project Template using Huff and Foundry.

## Getting Started w/ devtooligan Huff Project Template

Click "Use this template" on [GitHub](https://github.com/devtooligan/devtooligan-template) to create a new repository with this repo as the initial state.

Once you've cloned and entered into your repository, you need to install the necessary dependencies. In order to do so, simply run:

```shell
forge install
```

To test your contracts:

```shell
forge test
```


```ml
lib
├─ forge-std — https://github.com/foundry-rs/forge-std
├─ foundry-huff — https://github.com/huff-language/foundry-huff
scripts
├─ Contract.s.sol — Deployment Script
src
├─ Contract — A test contract
├─ SimpleStore  — A Simple Storage contract in Huff
test
└─ Contract.t — A test contract
└─ SimpleStore.t — Simple Storage tests
```


## License

[The Unlicense](https://github.com/huff-language/huff-project-template/blob/master/LICENSE)

## Acknowledgements

- [foundry-template](https://github.com/transmissions11/foundry-template)
- [femplate](https://github.com/abigger87/femplate)
- [nomad-xyz/monorepo](https://github.com/nomad-xyz/monorepo/)
- [huff-project-template](https://github.com/huff-language/huff-project-template)

## Disclaimer

_These smart contracts are being provided as is. No guarantee, representation or warranty is being made, express or implied, as to the safety or correctness of the user interface or the smart contracts. They have not been audited and as such there can be no assurance they will work as intended, and users may experience delays, failures, errors, omissions, loss of transmitted information or loss of funds. The creators are not liable for any of the foregoing. Users should proceed with caution and use at their own risk._
