# PegasusCrawler

## THE GraphQL automated testing tookit

PegasusCrawler is the most powerful automated testing toolkit for any SQL endpoint.

### Version 1.2 is out!!
NEW: Can search for endpoints for you using Escape Technology's powerful [Graphinder](https://github.com/Escape-Technologies/graphinder) tool. Just point it towards a domain and add the '-e' option and Graphinder will do subdomain enumeration + search popular directories for GraphQL endpoints. After all this PegasusCrawler will take over and work through each find. If the schema can not be introspected, you can supply it as a json file with the '-s' option.

It will run through and check if mutation is enabled, check for any sensitive queries available, such as users and files, and it will also test any easy queries it find to see if authentication is required.

I hope this saves you as much time as it has for me

## Usage
```bash
python PegasusCrawler.py -u https://pegasuscrawler.com/sobri3195/api -o <fileName> -a "<headers>"

██████╗░███████╗░██████╗░░█████╗░░██████╗██╗░░░██╗░██████╗
██╔══██╗██╔════╝██╔════╝░██╔══██╗██╔════╝██║░░░██║██╔════╝
██████╔╝█████╗░░██║░░██╗░███████║╚█████╗░██║░░░██║╚█████╗░
██╔═══╝░██╔══╝░░██║░░╚██╗██╔══██║░╚═══██╗██║░░░██║░╚═══██╗
██║░░░░░███████╗╚██████╔╝██║░░██║██████╔╝╚██████╔╝██████╔╝
╚═╝░░░░░╚══════╝░╚═════╝░╚═╝░░╚═╝╚═════╝░░╚═════╝░╚═════╝░
                                                                                            
 
```
The output option is not required and by default it will output to schema.json

### Example output:
<div></div>

### Requirements
- Python3
- Docker
- Install all Python dependencies with pip

<div></div>

Wordlist from [google-10000-english](https://github.com/first20hours/google-10000-english)


### TODO
- Add option for "full report" following the endpoint search where it will run clairvoyance and all other aspects of the toolkit on the endpoints found
- Default to "simple scan" to just find endpoints when this feature is added
- Way Future: help craft queries based of the shema provided

### Creator
Muhammad Sobri Maulana