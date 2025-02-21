
# 186 - [Multiple outdated Solidity versions in use](./Multiple%20outdated%20Solidity%20versions%20in%20use.md)

Outdated versions of Solidity are being used in all contracts. 

The compiler options in the truffle-config file specifies version 0.6.6, which was released on April 6, 2020. 

Throughout the codebase there are also different versions of Solidity being used.

### Recommendation:
As Solidity is now under a fast release cycle, consider using a more recent version of the compiler, such as version 0.7.6. 

In addition, to avoid unexpected behavior, consider specifying explicit Solidity versions in pragma statements.
___
## Slide Screenshot
![186.png](../../images/8.%20Audit%20Findings%20201/186.png)
___
## Slide Text
- OpenZeppelin Fei Protocol Finding L04
- Configuration
- Solidity Versions
- Outdated & Multiple
- Recent & Single & Fixed
___
## References
- [Youtube Reference](https://youtu.be/0J7KI4WGd0Q?t=253)
- [OpenZeppelin's Audit of Fei Protocol](https://blog.openzeppelin.com/fei-protocol-audit/)
___
## Tags
