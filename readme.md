# Rust Port Scanner

A multi-threaded port scanner written in Rust. It scans an IP address to detect open ports efficiently using concurrency.

## Features
- Multi-threaded for faster scanning
- Supports both IPv4 and IPv6
- Customizable number of threads

## Usage
```
Usage: <program> [IP_ADDRESS] [-j THREADS IP_ADDRESS]
  -j to specify the number of threads
  -h or -help to display this message
```

### Examples
#### Scan an IP address with the default number of threads (4):
```
cargo run --release 192.168.1.1
```

#### Scan an IP address with a specified number of threads:
```
cargo run --release -j 10 192.168.1.1
```

## Installation
### Prerequisites
- Install Rust ([Rust Installation Guide](https://www.rust-lang.org/tools/install))

### Build and Run
Clone the repository and compile the project:
```
git clone <repo-url>
cd <repo-folder>
cargo build --release
```
