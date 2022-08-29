# foundry-safe-script

A simple foundry script to deploy a Gnosis Safe to 

```
forge script src/GnosisDeployer.s.sol --sig "run()" --broadcast --fork-url $YOUR_RPC_HERE -t --sender $YOUR_SENDER_HERE --verify
```

## Instructions

1. Change the owners threshold

   
```solidity
address[] internal owners = new address[](3);
```

2. Set the owners of your choice

```solidity
owners[0] = address(0x0000000000000000000000000000000000000001);
owners[1] = address(0x0000000000000000000000000000000000000002);
owners[2] = address(0x0000000000000000000000000000000000000003);
```

3. Set a custom threshhold

```solidity
uint256 THRESHHOLD = 3;
```
