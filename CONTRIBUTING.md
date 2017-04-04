# Contributing

Docs are written (`.apib` files) in [API Blueprint](https://apiblueprint.org/) and rendered (`.html` files) with [Aglio](https://github.com/danielgtaylor/aglio). Select HTML files have been copied to a publicly-accessible URL on our FTP server.

## Setting Up Aglio
Install Aglio via NPM. You need Node.js installed and you may need to use `sudo` to install globally:

```bash
npm install -g aglio
```

## Helpful Aglio Commands

```bash
# Run a live preview server on http://localhost:3000/
aglio -i sending_an_email.apib --theme-template triple -s
```

```bash
# Use three-column layout
aglio -i sending_an_email.apib --theme-template triple -o sending_an_email.html
```

A list of all aglio commands can be found [here](https://github.com/danielgtaylor/aglio).

## API Folder structure

Files inside the `flows/` directory should be considered partner-publishable API documents. Each `.apib` file is rendered into a `.html` file by Aglio, which can be published. The rendered `.html` files should not be checked into the repository.


+ endpoints
  + rest_resource_name
    + endpoint.apib
    + get.apib
    + put.apib
    + post.apib
    + delete.apib
+ flows
  + flow_name.apib

## Helpful links
+ [aglio](https://github.com/danielgtaylor/aglio)
+ [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Here-Cheatsheet)
+ [Markdown Table Generator](http://www.tablesgenerator.com/markdown_tables#)

