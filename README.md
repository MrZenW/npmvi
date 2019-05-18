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
var express3 = require('@npmvi/express-3.0.0');
var express4 = require('@npmvi/express-4.0.0');
```


## Remove
```bash
$ cd ~/your_project
$ npmvi remove express@3.0.0
$ npmvi remove express@4.0.0
```