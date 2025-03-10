# logjuicer-web

This crate provides the `logjuicer-web` application to render report and access the [logjuicer-api](../web-service/).


## Usage

The application support the following SPA URL:

### Create a report: `/report/new?target=$URL`

### Compare two urls: `/report/new?target=$URL&baseline=$URL`

### Watch a report `/report/watch/$REPORT_ID`

### List reports: `/`

### Read report: `/report/$REPORT_ID`


## Contribute

Develop the web interface by first generating a report with:
`cargo run -p logjuicer-cli -- --report logjuicer.bin ...`. Then
run the

```ShellSession
trunk serve ./dev.html --address 0.0.0.0 --no-default-features
```
