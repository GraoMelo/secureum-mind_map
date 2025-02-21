# 111 - [Token only has one address](Token%20only%20has%20one%20address.md)
Tokens with multiple entry points for balance updates can break internal bookkeeping based on the address (e.g. `balances[token_address][msg.sender]` might not reflect the actual balance). (See [here](https://github.com/crytic/building-secure-contracts/blob/master/development-guidelines/token_integration.md#contract-composition))
___
## Slide Screenshot
![0111.png](../../images/5.%20Pitfalls%20and%20Best%20Practices%20201/111.png)
___
## Slide Text
- ERC20 Token Address
- Only One Address
- Multiple Addresses -> Multiple Balances -> Bugs
- Single Address
___
## References
- [Youtube Reference](https://youtu.be/WGM1SF8twmw?t=715)
___
## Tags