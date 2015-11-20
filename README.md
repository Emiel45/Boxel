Boxel
======
Boxel is a near real-time pixelator and Minecraft codec.

Usage
======
Boxel pixelates images, websites and video at 24fps.

Getting Started
================
Dependencies
-------------
Boxel has a third party dependecy PhantomJS and is used remotely. See this docker container for example https://hub.docker.com/r/wernight/phantomjs/

CLI Interface
--------------
Help messages are displayed throught the CLI:

.. code-block:: bash

  boxel --help

Streaming Interface
-------------------
Boxelizing in realtime requires a client websocket connection accepting
base64 encoded JPEG's and a wamp router. To start up the streaming server
make sure a wamp router url is specified in the CLI (default is localhost:9090).

For examples streaming video check out the boxel-demo app

Contribute
===========
If you'd like to contribute, check out the contributing guidelines.
