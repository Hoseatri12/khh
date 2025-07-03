haros Testnet Auto Bot
An automated bot for interacting with the Pharos Testnet, performing swaps, transfers, faucet claims, and daily check-ins to potentially qualify for airdrops.

Features ✨
Automated Swaps: Performs random swaps between WPHRS and USDC tokens
PHRS Transfers: Sends small amounts of PHRS to random addresses
Faucet Claims: Automatically claims testnet tokens from the faucet
Daily Check-ins: Completes daily check-in tasks for potential rewards
Proxy Support: Rotates proxies for each operation (if provided)
Multi-wallet Support: Processes multiple wallets sequentially
Prerequisites 📋
Node.js (v18 or higher)
npm or yarn
Pharos Testnet wallet with private keys
(Optional) Proxy list in proxies.txt
Installation ⚙️
Clone the repository:

git clone https://github.com/Hoseatri12/Pharos-Auto-Bot.git
cd Pharos-Auto-Bot
Install dependencies:

npm install
Create a .env file in the root directory with your private keys:

PRIVATE_KEY_1=your_first_private_key_here
PRIVATE_KEY_2=your_second_private_key_here
(Optional) Add proxies to proxies.txt (one per line):

http://user:pass@ip:port
socks5://user:pass@ip:port
Configuration ⚙️
The bot comes with default settings for the Pharos Testnet, but you can modify:

Network RPC URL in networkConfig
Contract addresses in tokens object
Swap amounts in performSwap function
Transfer amounts in transferPHRS function
Usage 🚀
Run the bot:

node index.js
The bot will:

Display a banner with project info
Load proxies (if available)
Process each wallet sequentially:
Claim faucet (if available)
Perform daily check-in
Execute 10 PHRS transfers
Execute 10 token swaps
Repeat every 30 minutes
Logging 📝
The bot provides color-coded logs:

✅ Success messages (green)
⚠️ Warnings (yellow)
❌ Errors (red)
🔄 Loading/process indicators (cyan)
➤ Step-by-step actions (white)
Important Notes ⚠️
This bot is for TESTNET use only
Never use mainnet private keys
The bot runs indefinitely until stopped (Ctrl+C)
All transactions use 0 gas price (testnet feature)
The bot includes random delays between operations
Support 💬
For issues or questions, please open an issue on GitHub.

Disclaimer ⚠️
This software is provided "as is" without warranties. Use at your own risk. The developers are not responsible for any losses or issues caused by using this bot.

License 📄
MIT License - See LICENSE file for details
