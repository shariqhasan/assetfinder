# assetfinder

Find domains and subdomains potentially related to a given domain.


## Install

If you have Go installed and configured (i.e. with `$GOPATH/bin` in your `$PATH`):

```
go install github.com/cybercdh/assetfinder@cybercdh
```

Otherwise [download a release for your platform](https://github.com/tomnomnom/assetfinder/releases).
To make it easier to execute you can put the binary in your `$PATH`.

## Usage

```
assetfinder [--subs-only] <domain>
```

## Sources

Please feel free to issue pull requests with new sources! :)

### Implemented
* jldc.me
* dnshistory.org
* Arquivo
* Maltiverse
* AlienVault
* dnsspy.io
* crt.sh
* certspotter
* hackertarget
* threatcrowd
* wayback machine
    * Need to use the `-w` flag to enable this as it sometimes is quite slow.
* dns.bufferover.run
* facebook
    * Needs `FB_APP_ID` and `FB_APP_SECRET` environment variables set (https://developers.facebook.com/)
    * You need to be careful with your app's rate limits
* virustotal
    * Needs `VT_API_KEY` environment variable set (https://developers.virustotal.com/reference)
* ~~findsubdomains~~
    * ~~Needs `SPYSE_API_TOKEN` environment variable set (the free version always gives the first response page, and you also get "25 unlimited requests") — (https://spyse.com/apidocs)~~
* riddler.io
    * Needs `RIDDLER_EMAIL` and `RIDDLER_PASS` environment variables to be set (https://riddler.io/)

### Sources to be implemented
* ~~http://api.passivetotal.org/api/docs/~~
* ~~https://community.riskiq.com/~~
* ~~https://riddler.io/~~
* http://www.dnsdb.org/
* https://certdb.com/api-documentation

## TODO
* Flags to control which sources are used
    * Likely to be all on by default and a flag to disable
* ~~Read domains from stdin~~
