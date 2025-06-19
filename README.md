
This project is a backend REST API service built using **Node.js**  that aggregates and exposes **EigenLayer restaking data**. It fetches data from **onchain sources and subgraphs**, stores it in **MongoDB**, and provides endpoints to access:

- Restakers and their stETH restake info
- Validator metadata and slashing events
- Reward breakdown for user addresses

 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/restakers` | List all restakers with amount and validator address |
| `GET` | `/validators` | List all validators with metadata, status, and slash history |
| `GET` | `/rewards/:address` | Return restaking rewards for a specific user wallet |

 Tech Stack

- **Node.js + Express** – REST API
- **MongoDB** – Data persistence
- **dotenv** – Secure configuration