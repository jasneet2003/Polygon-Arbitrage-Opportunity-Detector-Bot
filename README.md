# Polygon Arbitrage Opportunity Detector Bot

A simple and efficient bot built in Rust that detects potential arbitrage opportunities on the Polygon network by monitoring prices across multiple decentralized exchanges (DEXes).

---

### Demo

*(A 20-30 second screen recording showing the bot running is the most effective way to demonstrate your project.)*

![Demo GIF placeholder](https://via.placeholder.com/800x400.png?text=Record+a+GIF+of+the+bot+running+and+place+it+here)

---

### Key Features

- **Multi-DEX Monitoring:** Continuously fetches and compares token prices from QuickSwap and SushiSwap on the Polygon Mainnet.
- **Arbitrage Detection:** Identifies potential arbitrage opportunities by calculating the price difference for a given trade size.
- **Simulated Profit Calculation:** Calculates the estimated *net profit* after accounting for a simplified, configurable gas cost.
- **Database Logging:** Logs all profitable opportunities to a local SQLite database (`arbitrage_opportunities.db`) for persistent record-keeping.
- **Configurable:** All key parameters are managed in a simple `config.toml` file.
- **Asynchronous & Performant:** Built with Rust and Tokio for efficient, non-blocking network requests.

### Technology Stack

- **Language:** Rust
- **Blockchain Interaction:** `ethers-rs`
- **Asynchronous Runtime:** `Tokio`
- **Configuration:** `config-rs`
- **Database:** `rusqlite` (SQLite)
- **Network:** Polygon Mainnet

---

### Setup and Usage

This project requires a personal Polygon RPC URL to connect to the blockchain. **Setup is simple and takes less than 2 minutes.**

**1. Prerequisites:**
   - [Rust](https://www.rust-lang.org/tools/install) toolchain installed.
   - For Windows, [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/) are required.

**2. Clone the Repository:**
   ```bash

   git clone https://github.com/jasneet2003/Polygon-Arbitrage-Opportunity-Detector-Bot.git
