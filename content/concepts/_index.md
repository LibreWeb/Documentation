---
title: "Concepts"
weight: 2
description : "Learn about the concepts behind LibreWeb, especially useful if you are new to LibreWeb."
---

New to LibreWeb or the distributed web? Learn about the concepts.

## LibreWeb

LibreWeb (specifically LibreWeb Browser) is a fully decentralized open-source Web Browser.

Allowing you to browse and host your content on the new decentralized web/Internet. Powered by [IPFS](#ipfs).

Decentralization comes with many benefits, including but not limited to:

* **No censorship**. Because the data is stored in a decentralized manner across the world, governments and corporations can neither block nor censor any content.
* **No single-point-of-failure.** If a specific server/node is down, your data can be served by other nodes within the network.
* **Fast**. The nearest node can serve you the content, basically acting as a content delivery network (CDN), however then decentralized.

See also the [Project page](/project); if you want to learn more about the LibreWeb project.

### Markdown Syntax

LibreWeb is using [Markdown syntax](https://en.wikipedia.org/wiki/Markdown "External link") as the 'source-code' of your content/article/site/blog, similar to static-website generators like `Hugo` or `Jekyll`, however LibreWeb Browser does **not** need the conversion step from Markdown to HTML.

LibreWeb Browser parses & renders the Markdown documents directly, allowing the end-user to view content. Without HTML and JavaScript, websites are much cleaner and load faster. 

Regarding security, without JavaScript, WebRTC, PHP and/or SQL the web is a much safer place.  

This is a real content-first approach, which allows the user to change the look & feel of content, just like with e-books.

### Blockchain

LibreWeb is explicitly **NOT** using any Blockchain technology or based on a cryptocurrency. Because blockchain solutions can give huge scalability issues as well as an unnecessary bad influence on our climate.

Most importantly, there is no need to use this technology in order to create a decentralized Internet.

## IPFS

LibreWeb is built on top of [IPFS (InterPlanetary File System)](https://docs.ipfs.io/concepts/ "External link"), which is a distributed system for storing and accessing files, websites, applications, and data.

Making it possible to download a file from many locations that aren't managed by one organization:

* **Supports a resilient internet.** If someone attacks Wikipedia's web servers or an engineer at Wikipedia makes a big mistake that causes their servers to catch fire, you can still get the same webpages from somewhere else.
* **Makes it harder to censor content.** Because files on IPFS can come from many places, it's harder for anyone (whether they're states, corporations, or someone else) to block content. We hope IPFS can help provide ways to circumvent actions like these when they happen.
* **Can speed up the web when you're far away or disconnected.** If you can retrieve a file from someone nearby instead of hundreds or thousands of miles away, you can often get it faster. This is especially valuable if your community is networked locally but doesn't have a good connection to the wider internet.

![IPFS Stack](/concepts/images/ipfs-stack.jpg?width=50pc)
