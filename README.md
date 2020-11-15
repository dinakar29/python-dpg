# Deterministic Password Generator

Generate a deterministic password.

## Installation

```bash
wget https://raw.githubusercontent.com/dinakar29/python-dpg/master/dpg -O /usr/local/bin/dpg
```

## Usage

```bash
$ dpg --help

usage: dpg [-h] -u USERNAME -s SERVICE [-c COUNTER] -p PASSPHRASE

optional arguments:
  -h, --help            show this help message and exit
  -u USERNAME, --username USERNAME
                        Username
  -s SERVICE, --service SERVICE
                        Service
  -c COUNTER, --counter COUNTER
                        Counter
  -p PASSPHRASE, --passphrase PASSPHRASE
                        Passphrase
```

## Example

Generate a deterministic password for a `mysql` DB DB user called `db_user` by supplying the passphrase "`example`"

```bash
$ dpg -u db_user -s mysql -p example
Dv2ejROBbD6bV16
```
