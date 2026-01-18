# Casino Bot Documentation

This document explains how to run the bot and use all commands. Commands are grouped by game or feature.

## Setup

1) Install dependencies:
   npm install

2) Create a Discord application and bot:
   - Go to the Discord Developer Portal
   - Create a new application
   - Add a bot to the application
   - Copy the bot token
   - Copy the Application ID (Client ID)

3) Invite the bot to your server:
   - In OAuth2 -> URL Generator, select scopes: bot, applications.commands
   - Select permissions: View Channels, Send Messages
   - Open the generated URL and invite the bot

4) Create a .env file at the repo root:
   DISCORD_TOKEN=your_token_here
   DISCORD_CLIENT_ID=your_application_id
   ADMIN_USER_ID=your_discord_user_id (optional, for /grant)

5) Run the bot:
   npm run start

Slash commands can take some time to appear globally (up to about 1 hour).

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

- All games use fake currency stored in SQLite.
- Balances persist in data/casino.sqlite.
