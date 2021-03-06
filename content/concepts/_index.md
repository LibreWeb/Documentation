---
title: "Concepts"
weight: 2
description : "Learn about the concepts behind LibreWeb, especially useful if you are new to LibreWeb."
---

New to LibreWeb or the distributed web? Learn about the concepts.

## LibreWeb

LibreWeb - specifically the LibreWeb *Browser* - is a fully decentralized, free and open-source web browser.

Powered by [IPFS](#ipfs), it allows you to browse, create and host content on the new, decentralized Internet.

Decentralization comes with many benefits, including but not limited to:

* **Censorship resistent**. Because data is stored in a decentralized manner around the world, governments and corporations can neither block nor censor content.
* **No single-point-of-failure.** If a specific server or node fails, data is still served by other nodes within the network.
* **Fast**. The nearest node can serve content as part of a broad, decentralized, content delivery network (CDN). Many nodes are potentially available to serve the same content.

Visit the [Project page](/project) to learn more about the LibreWeb project.

### Markdown Syntax

![LibreWeb Settings](/concepts/images/libreweb-browser-settings.png#floatright)

LibreWeb uses simple [Markdown syntax](https://en.wikipedia.org/wiki/Markdown "External link") as the 'source-code' of your content (article, site or blog...). Similar to static website generators like `Hugo` and `Jekyll`. However, LibreWeb Browser does _not_ require conversion from Markdown to HTML.

LibreWeb Browser parses & renders Markdown documents *directly*, allowing end-users to view content without the need of HTML or JavaScript. This results in websites that are much cleaner and load faster. As an added benefit the LibreWeb browser has a 'content first' approach.

And without JavaScript, WebRTC, PHP or SQL websites becomes much safer to browse.

The LibreWeb browser allows visitors to easily change and customize their look & feel of the content - similar to e-book readers. See the screenshot on the right.


### Blockchain

LibreWeb explicitly does _not_ use Blockchain nor is it based on cryptocurrencies. It therefore avoids huge scalability issues and the unnecessary, negative impact upon the environment that's associated with these technologies. After all, neither is needed to create a fast, decentralized and censorship resistent Internet.

If blockchain technology is needed to solve a specific problem in the future, that is fine.

## IPFS

LibreWeb is built on top of [IPFS](https://docs.ipfs.io/concepts/ "External link") (InterPlanetary File System) - a distributed system for storing and accessing files, websites, applications, and data.

The underlying [IPFS](https://docs.ipfs.io/concepts/ "External link") technology makes it possible to download the same file from many locations, not managed by any single organization. 

[IPFS](https://docs.ipfs.io/concepts/ "External link"):

* **Supports a resilient Internet.** Imagine an [IPFS](https://docs.ipfs.io/concepts/ "External link") world in which Wikipedia's web servers suffer an attack or some other catastrophic failure. Users would still have access to the exact same webpages - served seamlessly from countless nodes elsewhere.
* **Makes it harder to censor content.** Because files on [IPFS](https://docs.ipfs.io/concepts/ "External link") can come from many places, it's much harder for governments, corporations or _anyone_ to block content. [IPFS](https://docs.ipfs.io/concepts/ "External link") is designed to circumvent censorship and other attacks.	
* **Can speed up the web when you're far away or disconnected.** Retrieving a file from nearby instead of hundreds or thousands of miles away often means getting it faster. This is especially valuable to communities that are networked locally but don't have good connections to the wider Internet. 

Learn more about [IPFS](https://docs.ipfs.io/concepts/ "External link") in the *IPFS Whitepaper* attached at the bottom of this page. 

![IPFS Stack](/concepts/images/ipfs-stack.jpg?width=50pc)

{{%attachments title="IPFS Documents" style="blue" pattern=".*(pdf)" /%}}
