# amplitude-browser-sdk-gtm-template
The amplitude GTM template with @amplitude/analytics-browser internal

# Difference from the official repo
Added support for a special `props` event property that will be parsed as a `query` from a URI. E.g.
```
"a=111&b=222" => { "a": "111", "b": "222" }
```
Each key from the parsed object will be added to the `eventProperties`
