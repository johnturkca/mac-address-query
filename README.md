# MAC Address Query

Dockerized network reconnaissance tool that queries MAC addresses via the macaddress.io API to resolve vendor/manufacturer information — useful for network asset identification and security assessments.

## Features
- Resolves MAC addresses to vendor/company names
- Docker and non-Docker execution modes
- CLI argument support
- Useful for network enumeration and asset discovery

## Tech Stack
`Python` `Docker` `Networking`

## Create an Account
Create a free account at https://macaddress.io and get your API key.

## Run with Docker
```bash
git clone https://github.com/johnturkca/mac-address-query.git
cd mac-address-query
docker-compose up
```

## Run Locally
```bash
python3 -m venv venv
source venv/bin/activate
pip3 install -r requirements.txt

# Query a MAC address
python3 mac_addr_query.py --addr=88:66:5a:35:5e:e2
```

## Example Output
```
MAC Address : 88:66:5a:35:5e:e2
Company     : Apple, Inc.
Address     : Cupertino, CA, US
```
