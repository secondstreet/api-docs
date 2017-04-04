# API Documentation

Documentation for the Second Street Platform API.

## Contributing

Docs are written (`.apib` files) in [API Blueprint](https://apiblueprint.org/) and rendered (`.html` files) with [Aglio](https://github.com/danielgtaylor/aglio). Select HTML files have been copied to a publicly-accessible URL on our FTP server.

### Setting Up Aglio
Install Aglio via NPM. You need Node.js installed and you may need to use `sudo` to install globally:

```bash
npm install -g aglio
```

### Helpful Aglio Commands

```bash
# Run a live preview server on http://localhost:3000/
aglio -i sending_an_email.apib --theme-template triple -s
```

```bash
# Use three-column layout
aglio -i sending_an_email.apib --theme-template triple -o sending_an_email.html
```

A list of all aglio commands can be found [here](https://github.com/danielgtaylor/aglio).

### API Folder structure
+ endpoints
  + rest_resource_name
    + endpoint.apib
    + get.apib
    + put.apib
    + post.apib
    + delete.apib
+ flows
  + flow_name.apib

### Helpful links
+ [aglio](https://github.com/danielgtaylor/aglio)
+ [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Here-Cheatsheet)
+ [Markdown Table Generator](http://www.tablesgenerator.com/markdown_tables#)


## API Flows

Files inside the `flows/` directory should be considered partner-publishable API documents. Each `.apib` file is rendered into a `.html` file by Aglio, which can be published. The rendered `.html` files should not be checked into the repository.

The following are internal descriptions of each file, useful for us to find or recognize our Flows, but not visible to the partner.

### Creating/Sending Single Message Campaigns (`sending_an_email.apib`)

Keywords: Explanations of message campaigns, single message campaigns, message campaign audiences, message versions, and scheduling messages

Published to: [http://images1.upickem.net/support/jake/api/sending_an_email.html](http://images1.upickem.net/support/jake/api/sending_an_email.html)

## Old-Style Documentation

The following documents follow the old style of simply putting everything into a Google Doc. That method should be considered deprecated, and the documents below should eventually be migrated to our API Blueprint.

### Single Sign-On

Keywords: Explanations of registration forms, form submissions, email address verifications, sessions, password resets, and retrieving user data

[Google Doc](https://docs.google.com/document/d/1UI9gMAWRMPR2u8EryumVXSAELJknuErIpoqq7lDyBsc/edit)

### Messaging Analytics

Keywords: Explanations of categorical charts, messaging statistics, message performance, a/b test performance, message demographic data

[Google Doc](https://docs.google.com/document/d/1Mb0h_b7SZCtRfhgc3Tge7Z9oa_YPLEUy9BAd2QxDl6A/edit)
