# crypto zombies demo

## contract inheritance

> ### library

- safemath.sol

> ### no inheritance

- ownable.sol
- erc721.sol

> ### inheritance

- zombiefactory.sol : ownable.sol
- zombiefeeding.sol : zombiefactory.sol (cryptoKitty interface, using safemath)
- zombiehelper.sol : zombiefeeding.sol 
- zombieattack.sol : zombiehelper.sol
- zombieownership.sol : zombieattack.sol, erc721 (using safemath)