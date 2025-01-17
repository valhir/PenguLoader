## Insecure options

> These options are intended for development purposes only and should be used at your own risk.

The following options allow you to bypass default UX security measures. To enable them, simply edit the `config` file:

```ini
[Main]

; Enable Chrome remote debugger using a specific port
;   to access the remote DevTools, just open http://localhost:PORT/json/list
;   you will see a list of URLs, then open the first one (http://localhost:PORT/...)
RemoteDebuggingPort=8888

; Disable all web security features
;   e.g. CORS requests and other web policies
DisableWebSecurity=1

; Ignore all error/invalid SSL certificates
;   i.e. requests to self-assigned SSL/untrusted HTTPS servers
IgnoreCertificateErrors=1

; Allow requests through a proxy (for debugging purposes only)
NoProxyServer=0

; Append custom Chromium command line arguments
ChromiumArgs=--disable-gpu --some-flag "--flag-with-value=some_value"
```
