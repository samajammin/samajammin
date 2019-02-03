# Samajammin.com

Here's my personal website. It's a simple, static site hosted on [IPFS](https://ipfs.io/) via [CloudFlare's gateway](https://www.cloudflare.com/distributed-web-gateway/):

[https://www.samajammin.com/](https://www.samajammin.com/)

## Deploy your own site to IPFS

1. [Download IPFS](https://docs.ipfs.io/introduction/install/#installing-from-a-prebuilt-package)

2. Connect your local IPFS node to the network

```
ipfs daemon
```

3. Add your content to IPFS

```
ipfs add -r /path/to/folder-with-your-content
```

That's about it! Read [this excellent walkthrough](https://developers.cloudflare.com/distributed-web/ipfs-gateway/connecting-website/) for detailed instructions, including how to set up a custom domain and SSL.

## Be a benevolent peer

One advantage of IPFS is that the more popular the content, the faster it will load. The more any content is shared across nodes, the more peer nodes that can serve it to our browsers.

If you add my site and other IPFS sites to your IPFS node, you will help me and and the IPFS community!

Follow these steps:

```
cd ~/ && mkdir ipfs-files # Create folder to download ipfs content
cd ipfs-files
ipfs get /ipns/www.samajammin.com
ipfs add -r www.samajammin.com
```

Thanks for your contribution to the peer-to-peer revolution :)
