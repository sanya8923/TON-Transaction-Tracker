# TON-Transaction-Tracker

This project is a payment service for TON (Telegram Open Network). It is written in Python and uses Flask for the web server, MongoDB for the database, and Pytoniq for interacting with the TON network.

## Features

- Retrieve new transactions from the TON network
- Store transactions in a MongoDB database
- Serve transactions over a REST API

## Installation

1. Clone the repository
2. Install the dependencies using Poetry:

```bash
poetry install
```

## Usage

1. Start the server:

```bash
python main.py
```

2. Access the transactions endpoint at `http://localhost:5001/transactions`

## Dependencies

- Python 3.12
- Flask 3.0.3
- Redis 5.0.4
- Requests 2.31.0
- Pydantic 2.7.1
- Pydantic-settings 2.2.1
- Pytoniq 0.1.37
- Motor 3.4.0
- Quart 0.19.5

## Configuration

Configuration is done through environment variables, which can be set in a `.env` file. The following variables are used:

- `pay_address`: The address to retrieve transactions from
- `db_cluster_name`: The name of the MongoDB cluster
- `database`: The connection string for the MongoDB database

## Contributing

Please feel free to submit issues and pull requests.

## License

This project is licensed under the MIT License.
