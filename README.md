# Port Scanner

A simple command-line port scanning tool written in Rust.

## Features

- Scan ports on a specified IP address using multiple threads.
- Customizable number of threads for parallel scanning.
- Command-line interface for easy usage.

## Usage

### Prerequisites

- Rust and Cargo installed on your system.

### Installation

Clone the repository:

```
git clone https://github.com/MRSKYWAY/port_scanner.git
cd port-scanner
```

### Usage

Run the port scanner with the following command:

```
cargo run -- [OPTIONS] IP_ADDRESS
```

Replace `[OPTIONS]` with the following command-line options:

- `-j THREADS`: Specify the number of threads for scanning ports.
- `-h` or `-help`: Display usage information and help message.

Replace `IP_ADDRESS` with the IP address you want to scan for open ports.

Example:

```
cargo run -- -j 4 192.168.1.1
```

This command will scan the IP address `192.168.1.1` with 4 threads for open ports.

### Example Output

```
Scanning ports on 192.168.1.1...
.......................................................
80 is open
443 is open
8080 is open
```

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.
