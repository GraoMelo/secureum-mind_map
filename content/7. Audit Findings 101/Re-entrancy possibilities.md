
# 99 - [Re-entrancy possibilities](./Re-entrancy%20possibilities.md)

There are several examples of interactions preceding effects: 
1. In the deposit function of the Collateral contract, collateral is retrieved before the user balance is updated and an event is emitted.
2. In the `_withdraw` function of the Collateral contract, collateral is sent before the event is emitted
3. The same pattern occurs in the `depositToInsuranceFund`, `depositEtherToInsuranceFund` and `withdrawFromInsuranceFund` functions of the Perpetual contract. 

It should be noted that even when a correctly implemented ERC20 contract is used for collateral, incoming and outgoing transfers could execute arbitrary code if the contract is also ERC777 compliant. 

These re-entrancy opportunities are unlikely to corrupt the internal state of the system, but they would affect the order and contents of emitted events, which could confuse external clients about the state of the system. 

### Recommendation:
Consider always following the “Check-Effects-Interactions” pattern or use `ReentrancyGuard` contract is now used to protect those functions
___
## Slide Screenshot
![099.png](../../images/7.%20Audit%20Findings%20101/099.png)
___
## Slide Text
- 
___
## References
- Youtube Reference
- Medium Risk severity finding from [OpenZeppelin’s Audit of MCDEX Mai Protocol](https://blog.openzeppelin.com/mcdex-mai-protocol-audit/)
___
## Tags
