# pwnloris
An improved slowloris DOS tool, it keeps attacking until the server starts getting exhausted.


## Detailed info

This script abuses the *CVE-2007-6750* vulnerability. This exploits works using just one machine by creating multiple threads and sending from each thread incomplete requests while keeping the collection alive thus using up all the resources of the server and making the website unreachable.


## Usage

Pass a host by IP or domain name and optionally a port and it will test your server. Another option is to add the `-t` or `--tor` argument to make every request go through tor.

    $ ./pwnloris.py host:port {-t/--tor}


## Installation

    $ pip install -r requirements.txt

