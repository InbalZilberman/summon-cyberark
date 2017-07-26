# summon-cyberark


CyberArk provider for [Summon](https://conjurinc.github.io/summon/).



## Install

Download the [latest release](https://github.com/conjurinc/summon-conjur/releases) and extract it to the directory `/usr/local/lib/summon`.

## Usage

Give summon-cyberark a variable name and it will fetch the relevant account's password for you and print the value to stdout.

```sh-session
$ summon-cyberark safe="SalesUS"&Object="DBPass"
8h9psadf39sdahfp98
```

## Configuration
The provider uses CCP in order to fetch the secret\variable.

Environment variables:
Appliance URLs
      CyberArk_CCP_URL for example: {{BaseURL}}/AIMWebService
