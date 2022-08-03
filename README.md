# Project neuland: RFC916 / http://securitytxt.org Radar of some German (state) assets
## Introduction

* Monitoring is built with https://monitoror.com
* https://monitoror.com/documentation/#tile-http-raw is used to fetch HTTP-Status and Contact information.
  * Current Regex is not perfect: ` "regex": "Contact:\\s*([^\\s]*)" `
  * TODO: Replace with a more strict one (email address)

Example monitoring for ` https://www.berlin.de/.well-known/security.txt `:

```
    {
      "type": "HTTP-RAW",
      "label": "Berlin",
      "params": {
       "url": "https://www.berlin.de/.well-known/security.txt", 
       "regex": "Contact:\\s*([^\\s]*)"
       }
```

## Contribute
Feel free to create a new dashboard by sending a pull request. You can use https://github.com/schniggie/neuland/blob/main/monitoror-federal.json as template.


## Dashboards

* [Federal states of Germany](https://seconduct.de/federal)
