# DC Enum

**DC Enum** is a command-line tool for enumerating Active Directory Domain Controllers (DCs) and listing domain users via LDAP queries.

It supports plaintext or SSL (LDAPS) connections and can authenticate using provided credentials or perform anonymous binds.

---

##  Features

- Enumerate users and attributes from one or multiple DCs
- Optional authentication with username and password
- Support for SSL/TLS connections
- Colored terminal output
- Easy-to-use CLI interface

---

##  Installation

Clone the repository and install locally using `pip`:

```bash
git clone https://github.com/killercd/dc-enum.git
cd dc-enum
pip install .
```



## Usage

```bash
usage: dc-enum [-h] -f FILE [-u USER] [-p PASSWORD] [--use-ssl]

DC Users Enumeration Tool

options:
  -h, --help            show this help message and exit
  -f FILE, --file FILE  File containing list of DC IPs (default: None)
  -u USER, --user USER  Username (default: None)
  -p PASSWORD, --password PASSWORD
                        Password (default: None)
  --use-ssl             Use SSL for connection (default: False)

Examples:
      # Basic usage with a DC IP list file
      python dc_enum.py -f dc_ips.txt

      # Specify username and password
      python dc_enum.py -f dc_ips.txt -u administrator -p 'P@ssw0rd'

      # Use SSL for secure connection
      python dc_enum.py -f dc_ips.txt -u administrator -p 'P@ssw0rd' --use-ssl

```