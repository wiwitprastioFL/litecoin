# FlashLight (FLG)

FlashLight is an experimental cryptocurrency, forked from Litecoin Core (MIT License).
This project is at an experimental stage: it has not been audited and has not been launched.

## Features

- Fair launch, no pre-mine
- Fixed supply of 250,000,000 FLG
- 1-minute block time
- Difficulty adjustment every 2 hours (120 blocks)
- Based on Litecoin Core (Scrypt, minable with CPU/GPU)
- Open source (MIT), parameters and genesis block are published

## Parameters

| Parameter | Value |
|---|---|
| Name / ticker | FlashLight / FLG |
| Total supply | 250,000,000 FLG (fixed) |
| Initial block reward | 50 FLG |
| Halving interval | every 2,500,000 blocks |
| Block time | 1 minute |
| Difficulty adjustment | every 2 hours (120 blocks) |
| Algorithm | Scrypt |
| P2P port | 9533 |
| Bech32 prefix | flg1... |
| Pre-mine | None |
| Data directory | ~/.flashlight |

## Genesis block

- Message: "FlashLight 09/Nov/2026 Cahaya baru untuk transaksi cepat"
- Timestamp: 1794182400
- nBits: 0x1e0ffff0
- Nonce: 885415
- Hash: 8f15feeda3dabbfc4b9c283136a65d55da27be0d81c93ee6ad84403a9a16a3e07

## Build

Requires Linux (Ubuntu) with 2 GB RAM or more.

    sudo apt-get install -y build-essential libtool autotools-dev automake pkg-config bsdmainutils python3 libevent-dev libboost-system-dev libboost-filesystem-dev libboost-test-dev libboost-thread-dev libfmt-dev libdb++-dev libdb-dev
    ./autogen.sh
    ./configure --without-gui --disable-tests --disable-bench --with-incompatible-bdb
    make -j2

## Disclaimer

- The modified code has not been security audited.
- A new network with low hashrate is vulnerable to 51% attacks.
- Shorter block times can increase orphaned blocks.
- No promises of profit or price increases are made.
- Use for learning and experimentation only.