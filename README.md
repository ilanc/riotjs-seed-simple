# Simple Seed

## Setup

You need a static file webserver to run the example. I use something called live-server which has live reload (which is nice because when you save a file in the IDE it reloads the page). Assuming you have node/npm installed you can install it like so:

```bash
npm install -g live-server
```

## Run

```bash
cd /path/to/index.html
live-server --port=8001
```

## RiotJs docs

- https://riot.js.org/guide/
- https://github.com/riot/examples

## Features of seed

- no build
- CDN global modules
- styling
  - google fonts
  - font-awesome

## Notes

- styling
  - included google fonts and font-awesome because most projects will need these
- prevent flash of unstyled content (optional)
  - index.html has `<body style="display: none;">` and then show it once app mounted / after init etc...
- tag specific css
  - see app.tag.html `<style>`
- debugging in chrome console
  - `console.log` at top of `app.tag.html`, click in devtools console to jump to source code
