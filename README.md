# NPMVI
**Node.JS Package Multiple Version Installer** is a  command tool, which allows you to install multiple versions for the same package in a project.

**NPMVI is NOT a replacement for NPM**


## Installation

```bash
$ npm install -g npmvi
```

## Usage
### Install a multi-version in your project
```bash
$ cd ~/your_project
$ npmvi install express@3.0.0
$ npmvi install express@4.0.0
```

### or install the multi-version that you installed before.

It's like the `npm install` command but it's used to install multi-version

```bash
$ cd ~/your_project
$ npmvi install
```

### Using the multi-version installed with NPMVI
```JavaScript
var express3NpmviObject = require('@npmvi/express-3.0.0');
var express4NpmviObject = require('@npmvi/express-4.0.0');

express3NpmviObject.index; // the original express3 module entrance
express3NpmviObject.name; // express
express3NpmviObject.version; // 3.0.0
express3NpmviObject.packageJSON; // express3 package.json
express3NpmviObject.isNPMVI; // true

express4NpmviObject.index; // the original express4 module entrance
express4NpmviObject.name; // express
express4NpmviObject.version; // 4.0.0
express4NpmviObject.packageJSON; // express4 package.json
express4NpmviObject.isNPMVI; // true
```


### Remove
```bash
$ cd ~/your_project
$ npmvi remove express@3.0.0
$ npmvi remove express@4.0.0
```