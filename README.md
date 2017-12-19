[![Build Status](https://travis-ci.org/exsilium/cloud9.svg?branch=master)](https://travis-ci.org/exsilium/cloud9)
[![Dependency Status](https://gemnasium.com/exsilium/cloud9.svg)](https://gemnasium.com/exsilium/cloud9)
[![Bitcoin donate button](https://img.shields.io/badge/bitcoin-donate-yellow.svg)](https://www.coinbase.com/checkouts/16wBMRsdZkNu6Vk7zQetX27aHLnvwusedz) 
"One-time donation to keep this fork alive"
 
# Cloud9 IDE v2 Alternative

As of 14th of February 2015 with a commit that can no longer be linked to, the upstream author Cloud9 IDE, Inc stated that the Cloud9 v2 would no longer be maintained. The original repository issue tracker was closed and notifications were given that the project is superseded by [Cloud9 v3 SDK](https://github.com/c9/core/) with some substantial changes in licensing terms driven by alignment of business goals. [exsilium/Cloud9 v2](https://github.com/exsilium/cloud9.git) is the maintained fork for the original Cloud9 IDE v2 that people grew to love. If it feels like these are limiting factors for you, you are welcome to try Cloud9 v2, which is licensed under GPL version 3.

This repository is alternative version of Cloud IDE v2 to support [Backend.AI](https://cloud.backend.ai) cloud PaaS (Platform as a Service).

## About Cloud 9 IDE v2

Cloud9 is an open source IDE built with [Node.JS] on the back-end and JavaScript/HTML5 on the client. The version available here runs on your local system. Cloud9 balances the power of traditional desktop IDEs with the simplicity and elegance of editors like TextMate and Sublime.

Cloud9 is built entirely on a web stack, making it the most hacker-friendly IDE today. Fork it, hack it, and if you think others would benefit, file a pull request on this repo or create an issue.

### Fork Extras

- Modern node support (NodeJS >= 0.10+)
- Up to date dependencies and compatibility fixes
- Terminal

### Features

  * High performance ACE text editor with bundled syntax highlighting support for JS, HTML, CSS and mixed modes.
  * Integrated debugger for [Node.JS] applications with views of the call stack, variables, live code execution and live inspector
  * Advanced JavaScript language analysis marking unused variables, globals, syntax errors and allowing for variable rename
  * Local file system is exposed through [WebDAV](http://en.wikipedia.org/wiki/WebDAV) to the IDE, which makes it possible to connect to remote workspaces as well
  * Highly extensible through both client-side and server-side plugins
  * Sophisticated process management on the server with evented messaging

## Browser Support

We support the newer versions of Chrome, Firefox and Safari.

## Installation and Usage

Requirements (>= 2.1.0):

  * NodeJS `>= 0.10.0`
  * g++-4.8

Install:

    git clone https://github.com/hephaex/cloud9v2a.git
    cd cloud9
    npm install

The above install steps create a `cloud9` directory with a `bin/cloud9.sh`
script that can be used to start Cloud9:

    bin/cloud9.sh

Optionally, you may specify the directory you'd like to edit:

    bin/cloud9.sh -w ~/git/myproject

Cloud9 will be started as a web server on port `-p 3131`, you can access it by
pointing your browser to: [http://localhost:3131](http://localhost:3131)

By default Cloud9 will only listen to localhost.
To listen to a different IP or hostname, use the `-l HOSTNAME` flag.
If you want to listen to all IP's:

    bin/cloud9.sh -l 0.0.0.0

## Open Source Projects Used

The Cloud9 IDE couldn't be this cool if it weren't for the wildly productive
[Node.JS] community producing so many high quality software.
Main projects that we use as building blocks:

  * [async.js] by [fjakobs]
  * [jsDAV] by [mikedeboer]
  * [connect] by [senchalabs](http://github.com/senchalabs)
  * [engine.io] by [LearnBoost](http://github.com/LearnBoost)
  * [smith.io](http://github.com/c9/smith.io) by [creationix](http://github.com/creationix) & [cadorn](http://github.com/cadorn)
  * [ace](http://github.com/ajaxorg/ace) by [fjakobs]
  * [apf](http://www.ajax.org) by [ajax.org]
  * and of course [Node.JS]!

Thanks to all developers and contributors of these projects!

[fjakobs]: http://github.com/fjakobs
[javruben]: http://github.com/javruben
[mikedeboer]: http://github.com/mikedeboer
[ajax.org]: http://www.ajax.org/
[async.js]: http://github.com/fjakobs/async.js
[jsDAV]: http://github.com/mikedeboer/jsdav
[connect]: http://github.com/senchalabs/connect
[engine.io]: http://github.com/LearnBoost/engine.io
[requireJS]: http://requirejs.org/
[Node.JS]: http://nodejs.org/

## License

The GPL version 3, read it at [http://www.gnu.org/licenses/gpl.txt](http://www.gnu.org/licenses/gpl.txt)
