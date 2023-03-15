# Bridge Smart Contract Information

The bridge contains two smart contracts: 

- Bridge1.sol which is deployed on Ethereum mainnet
- Bridge2.sol which is deployed on Ordinals Chain


One special feature to notice is that on Bridge1, WBTC (ERC20) will be accepted meanwhile on Bridge2, 
core coins (ordinals BTC) will be rewarded. The backend takes care of the difference between decimals

`    uint256 public lastId = 0;`
`
    uint256 public depositorsId = 0;
    `
    
The above two variables are checked in both smart contracts to find differences and issue bridge transfers. 
