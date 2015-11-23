Boxel
======
Boxel is a near real-time pixelator and Minecraft codec.

Usage
======
Boxel pixelates images, websites and video at 24fps.

You can use it to make funky pixelated artwork from existing assets to display wherever you like.
By default, Boxel creates a stream of PNG images along with JSON messages that describe the image.

Boxel was built to act as a codec for Minecraft. You can use the data it creates to build boxelized images,
websites and video from blocks on a Minecraft server.

We've created a client library that makes it easy to connect Bukkit compatible Minecraft plugins to a Boxel server.
Check it out [here](https://github.com/verizoncraft/Boxel-client)

Getting Started
================
Dependencies
-------------
Boxel depends on PhantomJS for rendering websites.
Installing on OSX with Homebrew is simple:
```bash
brew install phantomjs
```

Boxel expects to connect to Phantom remotely, so you should start it as below:
```bash
/usr/local/bin/phantomjs --webdriver=8910
```

We recommend using this Docker image to install and run your Phantom instance: [wernight/phantomjs](https://hub.docker.com/r/wernight/phantomjs/)

Boxel requires [Redis](http://redis.io) to send video data over PUB/SUB channels.
Redis can be installed via your package manager of choice:

```bash
# homebrew again
brew install redis

# or apt-get
sudo apt-get install redis-server
```

Installation
------------
After you've installed Phantom, install boxel and it's depencies like any other Python package:
```bash
# using pip
pip install -e https://github.com/VerizonCraft/Boxel.git#egg=boxel
```

Demo app
--------
The best place to start with Boxel is probably the [demo app](https://github.com/VerizonCraft/Boxel-demo).
It includes docker containers PhantomJS, Boxel, Redis, and an example web front-end that will get you a
running Boxel service with just a few commands.


Contribute
===========
If you'd like to contribute, check out the [contributing guidelines](https://github.com/VerizonCraft/Boxel/blob/master/CONTRIBUTING.md)

License
===========
This repository and its code are licensed under a BSD 3-Clause license, which can be found [here](https://github.com/VerizonCraft/Boxel/blob/master/LICENSE).

