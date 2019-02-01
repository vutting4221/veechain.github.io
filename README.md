Repository is dedicated for all BinanceChain Documentation

The main documentation is stored in `docs` folder, and developed with [Mkdocs](https://www.mkdocs.org/).

## How to Change the Docs

- install `mkdocs`
- In most times, you only need to add new pages with links on existing pages, such as index.md 
or *.md in `api-reference` fold. These files are all `markdown` format.
- Once you finish the editing, run `mkdocs serve` in the `Binance-Chain` directory, then you can 
preview the site via http://127.0.0.1:8000/. 

## Generating HTTP API Markdown

Use the following command to generate the Markdown documentation for the HTTP API:
`make build-markdown-http-docs`

## Generating RPC Docs Markdown

In bnc-tendermint, use the `make rpc-docs` command to generate the file, then copy the generated file over the existing `docs/api-reference/node-rpc.md`:
```bash
 $ cp ./index.html.md ../docs-site/docs/api-reference/node-rpc.md
 ```

## Generating JavaScript SDK Markdown

In javascript-sdk, use the `yarn build:docs` command to generate the file, then copy the generated file in `docs/jsdoc.md` over the existing `docs/api-reference/js-sdk/jsdoc.md`:
```bash
$ cp ./docs/jsdoc.md ../docs-site/docs/api-reference/js-sdk/jsdoc.md
```
