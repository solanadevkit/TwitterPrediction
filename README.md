# PANAGOT Twitter Prediction Market (Solana Devnet)

## Overview
PANAGOT transforms Twitter into a live, on-chain prediction market platform powered by Solana. Users can create, bet on, and resolve yes/no markets entirely via Twitter mentions and replies—no external site required.

## Features
- **Deposit SOL:** Users receive a unique, HD-derived Solana deposit address for their Twitter account. All deposits are tracked on-chain (Devnet).
- **Create Markets:** Anyone can create a yes/no prediction market by tweeting at @PANAGOT.
- **Betting:** Place bets by replying to market tweets with `@PANAGOT yes [amount]` or `@PANAGOT no [amount]`.
- **Balance Tracking:** The bot checks on-chain balances for each user’s deposit address.
- **Withdrawals:** Users can withdraw their balance by tweeting `@PANAGOT withdraw <amount> <solana_address>`.
- **All actions are performed natively on Twitter.**

## Workflow
1. **Deposit SOL**
   - Tweet: `@PANAGOT deposit`
   - The bot replies with your unique Solana deposit address and current balance.
2. **Create a Market**
   - Tweet: `@PANAGOT create [your yes/no question]`
   - The bot replies confirming market creation, with a Market ID and instructions to bet.
3. **Place a Bet**
   - Reply to the market tweet: `@PANAGOT yes 2` or `@PANAGOT no 1.5`
   - The bot checks your on-chain balance and replies with confirmation (if not rate-limited).
4. **Withdraw**
   - Tweet: `@PANAGOT withdraw <amount> <solana_address>`
   - The bot sends SOL to your specified address (Devnet).

## Notes
- All SOL actions are on Solana Devnet for testing.
- Twitter API rate limits may delay replies or confirmations.
- If the bot is rate-limited, actions are queued and retried after reset.

---


For questions or contributions, contact @Panagot on Twitter. 
