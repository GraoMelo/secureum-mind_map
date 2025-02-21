
# 112 - [`GovernorAlpha` proposals may be canceled by the proposer, even after they have been accepted and queued](./`GovernorAlpha`%20proposals%20may%20be%20canceled%20by%20the%20proposer,%20even%20after%20they%20have%20been%20accepted%20and%20queued.md)

`GovernorAlpha` allows proposals to be canceled via cancel. 

A proposer may cancel proposals in any of these states: Pending, Active, Canceled, Defeated, Succeeded, Queued, Expired.

### Recommendation:
Prevent proposals from being canceled unless they are in the Pending or Active states.
___
## Slide Screenshot
![112.png](../../images/8.%20Audit%20Findings%20201/112.png)
___
## Slide Text
- ConsenSys Audit Fei Protocol Finding 3.10
- Application Logic
- Proposal Cancellation & States Allowed
- Restrict Cancellation to Certain States
___
## References
- [Youtube Reference](https://youtu.be/IXm6JAprhuw?t=714)
- [ConsenSys's Audit of Fei Protocol](https://consensys.net/diligence/audits/2021/01/fei-protocol/#governoralpha-proposals-may-be-canceled-by-the-proposer-even-after-they-have-been-accepted-and-queued)
___
## Tags
