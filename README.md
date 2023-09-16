## .NET 8 RC1 SDK binding generation repro

Works with .NET 7 SDK (tested with (`7.0.400`)):
Fails with .NET 8 (tested with `8.0.100-rc.1.23455.8`)


`global.json` for repro:

```json
  "sdk": {
    "version": "7.0.100",
    "rollForward": "latestMinor",
    "allowPrerelease": false
  }
```


```json
  "sdk": {
    "version": "8.0.*",
    "rollForward": "latestMinor",
    "allowPrerelease": true
  }
```