# SubSniper

SubSniper is a fast and efficient Python-based subdomain finder designed to identify subdomains for a given domain. It supports multithreading for faster results and allows users to save the discovered subdomains to a file.

## Features

- **Multithreading**: Uses multiple threads to speed up the subdomain discovery process.
- **Custom Wordlists**: Accepts a wordlist of subdomains for testing.
- **Output to File**: Option to save discovered subdomains to a file.
- **Verbose Mode**: Prints discovered subdomains in real-time.
- **Customizable Threads**: Adjust the number of threads to optimize performance.

## Requirements

- Python 3.x
- `requests` module

You can install the required module using pip:

```bash
pip install requests
```


## Usage
To use SubSniper, run the script with the following options:

```sh
./subsniper.py [options] example.com
```

### Options
```sh
 -w  --wordlist  FILE: Wordlist file containing subdomains (required).
 -t  --threads   NUM: Number of threads to use (default: 100).
 -o  --output    FILE: File to save the discovered subdomains.
 -V  --verbose   Enable verbose output to print subdomains as they are found.
 -v --version    Display the version of the tool.
```


### Example Usage
+ Simple usage:

```sh 
./subsniper.py -w wordlist.txt example.com
```
+ With custom thread count and output file:

```sh
./subsniper.py -w wordlist.txt -t 50 -o results.txt example.com
```
+ Verbose mode
```sh
./subsniper.py -w wordlist.txt -V example.com
```


### Disclaimer
This tool is intended for educational purposes only. Please ensure you have permission from the target domain owner before running this tool against any domain.
