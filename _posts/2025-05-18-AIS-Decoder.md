---
title: "AIS decoder for Node-RED"
categories:
  - Blog
tags:
  - computing
---

Back in 2020 when COVID was on the rampage, I was messing about with a couple of bits of technology:

* [Node-RED](https://nodered.org/), a graphical system for implementing message-passing applications (called "flows"). It's a "low-code" tool, meaning that you don't need to be an expert coder - just connect functional blocks called "nodes" together graphically. It runs on [Node.js](https://nodejs.org/en), the well-known server-side Javascript environment.
* [AIS](https://en.wikipedia.org/wiki/Automatic_identification_system) or Automatic Identification System, a radio-based aid to marine navigation used throughout the maritime industry. Ships (and navigational aids) periodically send out AIS messages indicating their position, speed, course etc.

It struck me that it would be cool to feed AIS messages into Node-RED and see what could be done with them. So I wrote[^1] a new "node" for AIS, called [node-red-contrib-ais-decoder](https://github.com/chrisadie/node-red-contrib-ais-decoder). It's gradually got better over the years, and now reliably decodes virtually all AIS messages (including some really obscure ones).

There's also a demonstration "flow" called [node-red-contrib-flow-ais1](https://github.com/chrisadie/node-red-contrib-flow-ais1) which accepts information from an AIS receiver (eg a [RTL-SDR](https://www.rtl-sdr.com/about-rtl-sdr/) USB dongle) and displays a map with the location of nearby vessels. It's fun to mess with - check it out!

[^1]: I believe that nowadays I'm supposed to say "coded" rather than "wrote"!
