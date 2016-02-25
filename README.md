# api-docs
Documentation for the Second Street Platform API

---

## Current Location
[http://images1.upickem.net/support/jake/api/sending_an_email.html](http://images1.upickem.net/support/jake/api/sending_an_email.html)

## Setting Up aglio
Install aglio via NPM. You need Node.js installed and you may need to use `sudo` to install globally:

```bash
npm install -g aglio
```

## Helpful aglio Commands

```bash
# Run a live preview server on http://localhost:3000/
aglio -i sending_an_email.apib --theme-template triple -s

# Use three-column layout
aglio -i sending_an_email.apib --theme-template triple -o sending_an_email.html
```

A list of all aglio commands can be found [here](https://github.com/danielgtaylor/aglio).

## API Folder structure
+ endpoints
  + method
    + endpoint.apib
    + get.apib
    + put.apib
    + post.apib
    + delete.apib
+ flows
  + use_cases.apib

## Helpful links
+ [aglio](https://github.com/danielgtaylor/aglio)
+ [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Here-Cheatsheet)
+ [Markdown Table Generator](http://www.tablesgenerator.com/markdown_tables#)
