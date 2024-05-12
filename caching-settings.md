---
description: The Cloudflare cache settings which can be managed
---

# Caching Settings

You can manage the below cache settings by browsing to Settings -> Cloudflare -> Cache Settings

### Development Mode

When Development Mode is on, all requests will be passed to the origin server. This allows requests for your website to temporarily bypass our cache so you can verify changes made to cached content.

This is useful if you need to see changes immediately. Once enabled, Development Mode lasts for three hours and then automatically turns off.

**Note:** Unless you are making major changes to your website, we recommend using the Purge Individual Files option instead of turning on Development Mode. This is because Development Mode will cause all requests to go to your origin server, and increased requests to your origin server will temporarily raise your bandwidth and CPU usage.

### Caching Level

**What are Cloudflare’s** [**Caching Levels**](https://developers.cloudflare.com/cache/how-to/set-caching-levels)**?**

You can set Cloudflare’s CDN to cache [static content](https://developers.cloudflare.com/cache/about/default-cache-behavior) according to these levels:

* **No Query String:** Only delivers files from cache when there is no query string.
* **Ignore Query String:** Delivers the same resource to everyone independent of the query string.
* **Standard:** Delivers a different resource each time the query string changes.

We recommend using the Standard level. [Learn more about caching levels](https://developers.cloudflare.com/cache/how-to/set-caching-levels).

**Note:** By default, Cloudflare does not cache HTML content. You can create a Page Rule to [cache static HTML content](https://developers.cloudflare.com/cache/best-practices/customize-cache).

### Browser Cache TTL

**What does the Browser Cache TTL do?**

The Browser Cache TTL specifies how long cached files will remain in your visitor’s browser cache. This expiration time is what Cloudflare will set unless longer time periods are specified at your web server.

A longer expiration time ensures faster load times for repeat visitors. However, a longer expiration time also means slower update times if those files are modified.

[Learn more about Browser Cache TTL](https://developers.cloudflare.com/cache/about/edge-browser-cache-ttl#browser-cache-ttl).

**Note:** You can also increase the cache expiration by specifying a longer cache time on the origin server, or you can set a different Cache Expiration for a specific path or resource using the Page Rules app. Cloudflare will use whichever value is longer between your origin server cache headers and your Cloudflare setting

### Always Online™

**What does Always Online mean?**

If your server goes down, Cloudflare will serve your website’s most popular pages from our cache. For more information see [here](https://developers.cloudflare.com/cache/about/always-online).

Visitors viewing a cached page will receive a message informing them that they are in an offline browsing mode. As soon as your server comes back online, Cloudflare will move users back to regular browsing.

**Note:** If Cloudflare does not have the requested page in its cache, visitors will receive an error page letting them know the requested page is offline.

Refer to our support guide to [understand the limitations of Always Online](https://developers.cloudflare.com/cache/about/always-online).
