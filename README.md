<div align="center">

# Collider

A collider for the Atomicals protocol.

[![License](https://img.shields.io/badge/license-AGPL-blue.svg)](https://www.gnu.org/licenses/agpl-3.0.html)

![Mine](./static/mining.png)
Mine the Infinity (888888888.14) within 3 minutes (Lucky)
</div>

## Features

- Customizable verbosity level for detailed logging
- Support for both mainnet and testnet environments
- Configurable base fee for transactions
- Primary wallet and funding wallet management
- Ticker symbol specification
- Choice of mining algorithm (CPU or GPU or custom by your self)

## Getting Started

### Prerequisites

- Rust programming language (latest stable version)
- Cargo package manager

### Installation

#### Option 1: Using Pre-compiled Binaries

1. Download the pre-compiled binary for your operating system from the [releases page](https://github.com/nishuzumi/collider/releases).

2. Extract the downloaded archive to a directory of your choice.

3. Open a terminal and navigate to the directory where you extracted the binary.

#### Option 2: Building from Source

1. Clone the repository:
   ```shell
   git clone https://github.com/yourusername/collider.git
   ```

2. Change to the project directory:
   ```shell
   cd collider
   ```

3. Build the project:
   ```shell
   cargo build --release
   ```
4. The compiled binary will be located at `target/release/collider`.

### Usage

To run the Collider, use the following command:

```shell
./collider [OPTIONS]
```

#### Usage
```shell
Collier 0.1.0
A collier for atomicals.

USAGE:
    collider [FLAGS] [OPTIONS] --funding-wallet <funding-wallet> --primary-wallet <primary-wallet> --ticker <ticker>

FLAGS:
    -h, --help       Prints help information
    -V, --version    Prints version information
    -v, --verbose    Sets the level of verbosity

OPTIONS:
    -a, --api-url <api-url>                   [env: API_URL=]
    -b, --base-fee <base-fee>                 [env: BASE_FEE=]  [default: 50]
    -f, --funding-wallet <funding-wallet>     [env: FUNDING_WALLET=]
    -m, --miner <miner>                       [env: MINER=]  [default: cpu]
    -p, --primary-wallet <primary-wallet>     [env: PRIMARY_WALLET=]
        --testnet <testnet>                   [env: TESTNET=]
    -t, --ticker <ticker>                     [env: TICKER=]

```

You can set these environment variables in a `.env` file in the project root directory. The Collider will automatically load the variables from this file.

Example `.env` file:

```
API_URL=https://api.example.com
TESTNET=true
BASE_FEE=100
PRIMARY_WALLET=your_primary_wallet_address
FUNDING_WALLET=your_funding_wallet_private_key
TICKER=YOUR_TICKER
MINER=cpu
```

## Performance

The following table shows the performance benchmarks

| Device       | Commit Speed (ops/s) | Reveal Speed (ops/s) |
|--------------|----------------------|----------------------|
| Apple M3 GPU | 3M                   | 5M                   |
| Apple M3 CPU | 1M                   | 1.5M                 |

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License

This project is licensed under the GNU AFFERO GENERAL PUBLIC LICENSE.

## Acknowledgements

(Atomicals)[https://atomicals.xyz/] - The Atomicals protocol
Atomicalsir - For providing the foundation and inspiration for this project

## Contact

For any inquiries or questions, please contact [boxmrchen@fastmail.com](mailto:boxmrchen@fastmail.com).