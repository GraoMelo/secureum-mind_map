
# 53 - [Swapping on zero liquidity allows for control of the pool’s price](./Swapping%20on%20zero%20liquidity%20allows%20for%20control%20of%20the%20pool’s%20price.md)

Swapping on a tick with zero liquidity enables a user to adjust the price of 1 wei of tokens in any direction.

As a result, an attacker could set an arbitrary price at the pool’s initialization or if the liquidity providers withdraw all of the liquidity for a short time.

### Recommendation:
No straightforward way to prevent the issue. Ensure pools don’t end up in unexpected states. Warn users of potential risks.
___
## Slide Screenshot
![053.png](../../images/7.%20Audit%20Findings%20101/053.png)
___
## Slide Text
- ToB Audit Uniswap V3 Finding 8
- Application-logic
- Medium Severity
- Zero Liquidity
- Control Pool Price
- Design/Warn Appropriately
___
## References
- Youtube Reference
- Medium Risk severity finding from [ToB’s Audit of Uniswap V3](https://github.com/Uniswap/uniswap-v3-core/blob/main/audits/tob/audit.pdf)
___
## Tags
