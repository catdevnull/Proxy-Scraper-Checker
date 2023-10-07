# Proxy-Scraper-Checker
A command-line tool for scraping and checking HTTP and SOCKS5 proxies from the [checkerproxy.net proxies archive](https://checkerproxy.net/getAllProxy). By default, the working proxies are written to `proxies/http.txt` and `proxies/socks5.txt` according to the respective proxy type.

![image](https://github.com/Xewdy444/Proxy-Scraper-Checker/assets/95155966/91b55084-f82c-43d6-be29-6eaee1c8b23f)

## Installation

### Local
    $ cargo install --path .

### Rust Package Registry
    $ cargo install proxy-scraper-checker

## Usage
```
A command-line tool for scraping and checking HTTP and SOCKS5 proxies from the checkerproxy.net proxies archive

Usage: proxy-scraper-checker.exe [OPTIONS]

Options:
  -u, --url <URL>          The URL to check the proxies against [default: https://httpbin.org/ip]
      --tasks <TASKS>      The number of tasks to run concurrently for checking proxies [default: 512]
      --timeout <TIMEOUT>  The proxy request timeout in seconds [default: 30]
  -f, --folder <FOLDER>    The folder to save the working proxies to [default: proxies]
  -a, --anonymous          Only save anonymous proxies
      --http               Only save HTTP proxies
      --socks5             Only save SOCKS5 proxies
  -h, --help               Print help
```
