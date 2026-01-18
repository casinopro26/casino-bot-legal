# Casino Bot Documentation

This document explains how to run the bot and use all commands. Commands are grouped by game or feature.

## Add the Bot to Your Server

CasinoBot is installed from Discord’s Discovery / App Directory. You do not need to run any code locally.

1) Open the bot’s listing in the Discord App Directory.
2) Click Add to Server.
3) Choose your server and authorize the requested permissions.

After installing, slash commands are available in your server (they may take a short time to show).

## General Commands

- /help - list commands
- /bal - show your balance
- /claim - claim currency (1-hour cooldown)

## Economy

- /gift user:<user> amount:<amount> - gift currency to another user
- /grant user:<user> amount:<amount> - admin-only grant (requires ADMIN_USER_ID)

## Slots

- /slots bet:<amount> - spin the slots
- /slot bet:<amount> - alias for slots

## Horse Race

- /race bet:<amount> horse:<1-6> - bet on a horse

## Ride the Bus

- /rtb bet:<amount> - start a round
- /rtbcashout - cash out after a win
- /rtbcancel - cancel and forfeit
- /red - choose red
- /black - choose black
- /higher - choose higher
- /lower - choose lower
- /inside - choose inside
- /outside - choose outside
- /spades - choose spades
- /hearts - choose hearts
- /diamonds - choose diamonds
- /clubs - choose clubs

## Blackjack

- /blackjack bet:<amount> - start a blackjack hand
- /hit - take another card
- /stand - hold and resolve
- /double - double down (first two cards only)
- /blackjackcancel - cancel and forfeit

## Poker (3 Card Poker)

- /poker ante:<amount> - start a hand
- /play - match ante and resolve
- /fold - fold the hand
- /pokerstatus - show current hand
- /pokercancel - cancel and forfeit

## Notes

- All games use fake currency only.
- Use /bal to check your current balance at any time.
