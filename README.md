Surly2
======

<br>
node -v
<br>
v14.15.4
<br>
npm -v
<br>
7.6.0
<br>
<br>
<br>
<br>
<br>
<br>


> **surly** *adjective*
>
>  1. bad-tempered and unfriendly

Surly2 is a half-complete node.js AIML interpreter with a bad attitude.

Surly2 is a remake from the ground up of [Surly](http://github.com/mrchimp/surly) using Node 5 and using as much asynchronicity as possible.


Status
======

Actually works quite well so far but not everything is implemented. Even so, I wouldn't try using it for anything serious quite yet. Check out `COVERAGE.md` for full details.


Requirements
============

[Node.js](https://nodejs.org/)


Installation
============

 1. Acquire code
 2. `npm install`


Config
======

Config files are found and read by [rc](https://www.npmjs.com/package/rc). Check the "Configuration File Formats" section of the `rc` readme for more instructions. Any flag shown in `node cli.js --help` can be set in the options file.


1. Create a config file.

        ~/.surly2rc

2. You can set defaults for any argument. See `xmpp --help` for a list of available arguments.

        {
            "brain": "/path/to/aiml/files",
            "username": "surlybot@gmail.com",
            "password": "hunter2",
            "host": "talk.google.com",
            "port": "5222"
        }

3. Then just run it - no arguments!

        node xmpp.js
Usage
=====

1. `node cli.js`
2. Talk to Surly.
3. Type `exit` to exit.

Or chat over XMPP

1. Set up a config file (see above) with XMPP details `username`, `password`, `host` and `port`.
2. `node xmpp.js`
3. You can't add contacts yet. You'll have to do that yourself somehow.

Debugging
=========

Surly uses the [debug](https://www.npmjs.com/package/debug) npm package for debugging. E.g.

    DEBUG=surly2 node cli.js

Thanks
======

* [Richard Wallace](http://www.alicebot.org/bios/richardwallace.html), creator of AIML and AliceBot.
* Noel Bush, author of the well written, if jargon-dense, [AIML v1.0.1 spec](http://www.alicebot.org/TR/2001/WD-aiml/).
