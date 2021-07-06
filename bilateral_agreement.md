#  Bilateral Agreement

![Payer Profit](image/payers/payer_profit.png)

## Counterparties

A Yield Swap is a bilateral agreement, a [Future-Contract], between so-called Payers and Receivers. Payers is said to "buy" or go "long" the floating yields, and the Receiver is said to "sell" or go "short" the floating yield.

Whereas Payers bet on rising floating yields, Receivers bet on the opposite.

A user of the Yield Swap Protocol can take either of these roles whereas the so-called Liquidity Pool (see section below) of the Yield Swap Protocol will take the other.

## Terms

The main terms of a Yield Swap are:

1. underlying floating yield (say the interest from aUSDC),
2. notional value (say USDC 1000),
3. tenor (say 10 days), and
4. fixed interest rate (say 5% p.a.).

## Cash Flows

At maturity, the Payer pays the fixed-interest rate (applied to the notional for the tenor) to the Receiver, and in return receives the actual realized floating yield (applied to the notional for the tenor) from the Receiver.

## Profit and Loss

In case the realized (accumulated) floating yield is higher than the fixed yield, the Payer makes a profit (Receiver makes a loss), and otherwise the Payer makes a loss (Receiver makes a profit).

## Settlement

Only the net amount is settled at maturity, i.e., the difference between the realized floating and fixed interest rate (applied to the notional during the tenor).

## Margin Account

In order to reduce settlement risk, both Payers and Receivers must maintain sufficient collateral in a margin account.

## Automated Market Maker

The Yield Swap Protocol uses an Automated Market Maker (AMM) to always offer users a fixed interest yield for Giver and Receiver swaps.

## Liquidity Pool

The Liquidity Pool (LP) is counterparty to each and every Yield Swap. Funders of the LP are referred to a Liquidity Stakers (LS), and participate in the profit and loss of the Liquidity Pool.

[Future-Contract]: ./glossary.md[Future-Contract]
