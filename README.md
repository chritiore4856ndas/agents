# Agents

A fork of [Polymarket/agents](https://github.com/Polymarket/agents) — autonomous trading agents for Polymarket prediction markets.

## Overview

This project provides a framework for building and running automated agents that interact with Polymarket prediction markets. Agents can analyze market data, make trading decisions, and execute trades autonomously.

## Features

- Autonomous market analysis and trading
- Configurable agent strategies
- Integration with Polymarket API
- Docker support for easy deployment

## Requirements

- Python 3.10+
- Docker (optional)

## Setup

### 1. Clone the repository

```bash
git clone https://github.com/your-username/agents.git
cd agents
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Configure environment

Copy the example environment file and fill in your credentials:

```bash
cp .env.example .env
```

Edit `.env` with your Polymarket API keys and other configuration.

### 4. Run an agent

```bash
python -m scripts.run_agent
```

## Docker

Build and run with Docker:

```bash
docker build -t agents .
docker run --env-file .env agents
```

## Project Structure

```
agents/
├── scripts/         # Entry point scripts
├── src/
│   ├── agents/      # Agent implementations
│   ├── markets/     # Market data and analysis
│   └── utils/       # Shared utilities
├── tests/           # Test suite
├── .env.example     # Environment variable template
└── requirements.txt # Python dependencies
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

MIT
