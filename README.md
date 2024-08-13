
# 🚀 Make Trading Easy and Profitable with Sniper-Bot-Solana! Start Building Your Fortune Today! 💰


## 🎯 Sniper-Bot-Solana

the **sniper-bot-solana**! is an advanced trading tool designed for the Solana blockchain's Raydium decentralized exchange. This bot is built to automatically identify and purchase tokens from newly created liquidity pools on Raydium, providing users with the ability to capitalize on fresh trading opportunities faster than manual methods or the Raydium UI.

## 🚀 Key Features

- **WSOL Support**: Uses WSOL (Wrapped SOL) for trading; SOL is needed for transaction fees.
- **Auto-Sell**: Automatically sells tokens based on take profit and stop loss settings.
- **Configurable Take Profit/Stop Loss**: Default settings are 50% take profit and 30% stop loss, adjustable as needed.
- **Sniping List**: Target specific tokens by adding them to a snipe list.
- **Liquidity Checks**: Verifies token liquidity, including checks for burns, locks, and renounced mints.
- **Fast Execution**: Executes trades faster than the Raydium UI for timely opportunities.

## 📈 Take Profit & Stop Loss

- **Take Profit**: Default is 50%. Modify in the configuration if needed.
- **Stop Loss**: Default is 30%. Adjust according to your risk management preferences.

## 🔄 Auto-Sell

By default, auto-sell is enabled. To customize:

1. Set `AUTO_SELL` to `false` to disable auto-sell.
2. Adjust `MAX_SELL_RETRIES` to define the number of sell retries.
3. Set `AUTO_SELL_DELAY` to control the delay before selling. A delay of 0 means immediate selling (which may not guarantee profit).

## 🎯 Sniping List

To focus on specific tokens:

1. Set `USE_SNIPE_LIST` to `true`.
2. Add token mint addresses to the `snipe-list.txt` file, one address per line.
3. Update the list during script runtime; the script will refresh based on the `SNIPE_LIST_REFRESH_INTERVAL`.

## 🛠️ Setup Instructions

### Option 1: Local Machine

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/AhmedRabby2002/Solana-Raydium-Sniper-Bot.git
   ```
   Or download the ZIP file from GitHub.

2. **Install Node.js**:
   Download from [nodejs.org](https://nodejs.org/en).

3. **Install Dependencies**:
4. 
   Navigate to the project directory and run:
   ```bash
   npm install
   ```

5. **Convert SOL to WSOL**:

1. **Create a New Solana Wallet**:
   - If you don’t have a Solana wallet, you can create one using [Phantom Wallet](https://phantom.app/), a popular and user-friendly option.

2. **Transfer SOL**:
   - Transfer some SOL to your Phantom Wallet.

3. **Convert SOL to USDC or WSOL**:
   - Use [Jupiter](https://jup.ag/) to convert SOL to USDC or WSOL, depending on your needs.
   - 
![jupiterwrap (1)](https://github.com/user-attachments/assets/a6c9322a-cf3d-44a3-a2df-c14b41cc0dc4)

7. **Install Dependencies**:
   
   ```bash
   npm install
   ```

### Option 2: Using Gitpod (No Local Machine Required)
1. **Open Gitpod**:
   Click on the following link to open this project in Gitpod: [Open in Gitpod](https://gitpod.io/#https://github.com/SolanaNinja/sniper-bot-solana).

2. **Gitpod Workspace Setup**:
   - Gitpod will automatically set up a development environment for you in the cloud.
   - Once the workspace is ready, Gitpod will open a terminal where you can install dependencies and configure the script.

3. **Install Dependencies**:
   In the Gitpod terminal, run:
   ```bash
   npm install
   ```

4. **Configure the Script**:
   - Gitpod should have already copied `.env.copy` to `.env`. If not, you can manually copy it.
   - Update `.env` with your private key, RPC endpoints, and other settings.

5. **Convert SOL to WSOL**:
   Ensure you have a way to convert SOL to WSOL as Gitpod won’t have access to external services directly. You might need to use a web-based service or API for this.



## ⚙️ Configuration
1. Configure the script by updating `.env.copy` file (**remove the .copy from the file name when done**).
2. `PRIVATE_KEY` (your wallet private key)
3. `RPC_ENDPOINT` (https RPC endpoint)
4. `RPC_WEBSOCKET_ENDPOINT` (websocket RPC endpoint)
5. `QUOTE_MINT` (which pools to snipe, USDC or WSOL)
6. `QUOTE_AMOUNT` (amount used to buy each new token)
7. `COMMITMENT_LEVEL` 
8. `CHECK_IF_IS_BURNED` (liquidity burn check)
9. `CHECK_IF_IS_LOCKED` (liquidity lock check)
10. `USE_SNIPE_LIST` (buy only tokens listed in snipe-list.txt)
11. `SNIPE_LIST_REFRESH_INTERVAL` (how often snipe list should be refreshed in milliseconds)
12. `CHECK_IF_MINT_IS_RENOUNCED` (script will buy only if mint is renounced)
13. `MIN_POOL_SIZE` (script will buy only if pool size is greater than specified amount)
14. `TAKE_PROFIT=50` (in %)
15. `STOP_LOSS=30` (in %)
16. `BIRDEYE_API_KEY=` (TP/SL, Burn/Lock) generate here : https://docs.birdeye.so/docs/authentication-api-keys

    
![env](https://github.com/user-attachments/assets/b6a16dfc-2ee9-48c7-b871-1c9a2f0ce2c6)

**RPC Recommendation**: Try [Helius Labs](https://www.helius.xyz) for a reliable RPC service. Sign up for free and use the referral code `3wISAeRX8K` to get 5,000,000 free credits on the paid plan.

6. **Run the Script**:
   In the terminal, start the script by typing :
   
   ```bash
   npm run start
   ```
   ![preview](https://github.com/user-attachments/assets/06318090-ca4d-4f5b-b055-9c1049d14345)

## ❓ Common Issues

- **Empty Transactions**: Change commitment level to "finalized".
- **Unsupported RPC Node**: Use supported nodes like Shyft, Helius, or Quicknode.
- **No Token Account**: Ensure your wallet has a WSOL token account by swapping SOL to WSOL.

## 📝 Notes

- **Testing**: Run the bot for a few hours to evaluate its performance before full-time use.

## 📈 Future Plans

- **Notifications**: Integrate notifications via Discord or Telegram to keep you updated on bot activity and trading events. Stay tuned for updates on how to configure these notifications.
- **Docker Integration**: Introduce Docker support to simplify deployment and management of the bot in various environments. Instructions will be provided once Docker support is added.

## 📧 Contact

For support or inquiries about the premium version, please email: [omarleoni2000@gmail.com](mailto:omarleoni2000@gmail.com)

Here’s a revised version of your donation message with emojis and a more prominent look:

---

# 💖 Support Our Project! 💖**

Help us continue our work by making a donation to the Solana address below. Every contribution counts and is greatly appreciated!

# 🚀 Solana Address:
# 3nNESw5TypzEY1982zAJnokwX8x2dGij99M39E2meRRn

Thank you for your support! 🙏

**Future Plans**: We're looking to expand the team and potentially integrate AI into the project. If you're interested in contributing or have ideas, please get in touch!

