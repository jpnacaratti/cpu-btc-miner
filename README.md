# CPU Bitcoin miner

[![Python 3.10.14](https://img.shields.io/badge/Python-3.10.14-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Stratum protocol](https://img.shields.io/badge/protocol-Stratum-orange)](https://en.bitcoin.it/wiki/Stratum_mining_protocol)
[![MIT License](https://img.shields.io/badge/license-MIT-yellow.svg)](LICENSE)
[![GitHub last commit](https://img.shields.io/github/last-commit/jpnacaratti/cpu-btc-miner)](https://github.com/jpnacaratti/cpu-btc-miner)

A simple Bitcoin miner implemented in pure Python, designed for CPU mining with support for pool mining via the Stratum protocol. This miner allows you to connect to a mining pool and participate in the Bitcoin network by contributing your CPU's computational power to help process transactions and secure the network.

This miner only supports the low difficulty public pool: https://web.public-pool.io/#/

**Note:** This project was developed just for fun and learning. Its focus is not to generate profits, and mining will not be financially rewarding.

## Instructions

Open `main.py` and you'll see 6 variables to change:
- `POOL_HOST`, `POOL_PORT`, `POOL_PASS`: Pool configuration. It is not recommended to change these, as the miner only supports public-pool.io.
- `BTC_ADDRESS`: Address of your Bitcoin wallet.
- `WORKER_NAME`: Name of the worker that will mine.
- `SUGGESTED_DIFFICULTY`: Difficulty for finding valid shares.

Change the variables as needed, especially the `BTC_ADDRESS` to ensure you are rewarded correctly.

Start the miner on your PC just running the `main.py` script.
```
python main.py
```

**Note:** This project was written in Python 3.10.14 so I cannot guarantee it works on any other version.

## Roadmap

- [x] Add hashrate for each individual thread
- [ ] Add compatibility with other pools
- [ ] Add handling in case the user is not connected to Wifi
- [ ] Add combined hashrate for all threads
- [ ] Compatibility for cases where the pool does not have a version mask

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
