# Speculating on Falling Yields

Jon wants to speculate on falling aUSDC yields.
He believes that the current aUSDC deposit rate of `2.1% p.a.` will drop in the next 10 days and effectively be at `0.3% p.a.`

Jon goes to Yield Swap, where he is offered the following deal:
* he receives a fixed yield of `2% p.a.`
* he pays whatever the effectively realized aUSDC rate will be during the next 10 days


If Jon is right and aUSDC turns out to be `0.3% p.a.`, then:

| Jon receives               | Jon pays                   | Net                         |
| -------------------------- | -------------------------- | --------------------------- |
| `+0.055% = +2% * 10/365`   | `-0.008% = -0.3% * 10/365` | `+0.047% = 0.055% - 0.008%` |

Jon wants to close the deal for a notional of `1,000,000 USDC`, meaning that if everything goes as expected he will earn: `470 USDC = 0.047% * 1,000,000 USDC`.

In order to close the deal, Jon needs to pledge collateral to his Yield Swap margin account. The required collateral is `2,740 USDC = 10% * 1,000,000 USDC * 10/365` (where `10%` is Yield Swap’s maximum expected relative yield change for the next 10 days).


### Scenario A: Jon was right
The realized aUSDC rate is `0.3% p.a.` and Jon receives `470 USDC` as well as the original collateral of `2,739 UDSC`.
Effectively Jon made a return of `17.15% = 470 USDC / 2,740 USDC`.

### Scenario B: Jon was wrong
The realized aUSDC rate is `2.5% p.a.`, this means:

* he receives: `+548 USDC = +2% * 1,000,000 USDC * 10/365`
* he pays: `-685 USDC = -2.5% * 1,000,000 USDC * 10/365`

On a net basis, Jon loses: `-137 USDC = +548 USDC - 685 USDC`.

So he receives back `2,603 USDC = 2,740 USDC - 137 USDC` from his originally posted collateral,  effectively resulting in a return of `-5% = -137 USDC / 2,740 USDC`.
