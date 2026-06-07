# Wi-Fi QR Code Generator

<img src="docs/images/qr.png" align="right"/>

[![Test Status](https://github.com/Akashdeore15/wifiqr/workflows/Test/badge.svg)](https://github.com/Akashdeore15/wifiqr/actions?query=workflow%3ATest)
[![PkgGoDev](https://pkg.go.dev/badge/github.com/Akashdeore15/wifiqr)](https://pkg.go.dev/github.com/Akashdeore15/wifiqr)
[![Go Report Card](https://goreportcard.com/badge/github.com/Akashdeore15/wifiqr)](https://goreportcard.com/report/github.com/Akashdeore15/wifiqr)
[![codecov](https://codecov.io/gh/Akashdeore15/wifiqr/branch/main/graph/badge.svg)](https://codecov.io/gh/Akashdeore15/wifiqr)

Create a QR code with your Wi-Fi login details.

Use Google Lens or other application to scan it and connect automatically.

## Installation

Choose a binary from the [releases](https://github.com/Akashdeore15/wifiqr/releases).

### Build from Source

Download and [install Go](https://golang.org/doc/install).

Install the application:

```sh
go install github.com/Akashdeore15/wifiqr/cmd/wifiqr@latest
```

See the [go install](https://go.dev/ref/mod#go-install) instructions for more information about the command.

## Usage

```text
$ wifiqr --help
wifiqr is a WiFi QR code generator

It is used to create a QR code containing the login details such as
the name, password, and encryption type. This QR code can be scanned
using Google Lens or other QR code reader to connect to the network.
It is Android and iOS compatible.

If the options necessary for creating the QR code are not given on
the command line, the user will be prompted for the information.

Usage:
  wifiqr [flags]

Flags:
  -h, --help              help for wifiqr
      --hidden            Hidden SSID
  -k, --key string        Wireless password (pre-shared key / PSK)
  -o, --output string     PNG file for output (default stdout)
  -p, --protocol string   Wireless network encryption protocol (WPA2, WPA, WEP, NONE). (default "WPA2")
  -s, --size int          Image width and height in pixels (default 256)
  -i, --ssid string       Wireless network name
  -v, --version           version for wifiqr
```

## Usage Example

```sh
./wifiqr --ssid some_ssid --key 1234 --output qr.png --size 128
```

## License

MIT

## Maintainer

Akash Deore is a Cloud Security and Platform Engineer with over 4 years of experience in enterprise security delivery and cloud infrastructure automation. He maintains this project to provide a reliable and secure utility for network credential sharing.

GitHub: [Akashdeore15](https://github.com/Akashdeore15)
LinkedIn: [Akash Deore](https://www.linkedin.com/in/akash-deore)
Email: akashdeore1999@gmail.com