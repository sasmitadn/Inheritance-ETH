## Inheritance Balance Smart Contract

Public created plan and deposit into smart contract, set the timer for ping every X days. After countdown go to 0, beneficiaries can claim amount that has been set in the plan.

## Development

- Add contract address based on chain id on CONTRACT_ADDRESSES
- contract.json must be contain compile json data from e.g hardhat

## Cara Running

1. npx hardhat note
2. npx hardhat compile (ketika open kode yang akan dicompile)
3. npx hardhat ignition deploy ignition/modules/Inheritance.ts --network localhost 

Jika gagal, delete folder ignition/deployments dan cache

## Cara Running dari Remix IDE

1. Deploy ke network dev hardhat
2. copy abi ke abi.json
3. copy contract address

Enjoy!

## Changes

- Remove beneficiary
- Fix bug cancel plan will return all available asset
- Withdrawl with custom amount
- UI/UX Update