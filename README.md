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
git clone https://github.com/yourname/dc-enum.git
cd dc-enum
pip install .

