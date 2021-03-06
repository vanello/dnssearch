# dnssearch

This software is a subdomain enumeration tool.

[![baby-gopher](https://raw.githubusercontent.com/drnic/babygopher-site/gh-pages/images/babygopher-badge.png)](http://www.babygopher.org) 

## Purpose

dnssearch takes an input domain ( `-domain` parameter ) and a wordlist ( `-wordlist` parameter ), it will then perform concurrent DNS requests
using the lines of the wordlist as sub domains eventually bruteforcing every sub domain available on the top level domain.

It supports a custom file extension ( `-ext`, default to `php` ) and other optional arguments:

    Usage of ./dnssearch:
      -consumers int
            Number of concurrent consumers. (default 8)
      -domain string
            Base domain to start enumeration from.
      -wordlist string
            Wordlist file to use for enumeration. (default "names.txt")

## Compilation

    go get github.com/evilsocket/dnssearch
    cd dirsearch
    go build -o dnssearch main.go

## License

This project is copyleft of [Simone Margaritelli](http://www.evilsocket.net/) and released under the GPL 3 license.

