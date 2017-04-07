# api documentation for  [simplecrawler (v1.1.1)](https://github.com/cgiffard/node-simplecrawler)  [![npm package](https://img.shields.io/npm/v/npmdoc-simplecrawler.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-simplecrawler) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-simplecrawler.svg)](https://travis-ci.org/npmdoc/node-npmdoc-simplecrawler)
#### Very straightforward, event driven web crawler. Features a flexible queue interface and a basic cache mechanism with extensible backend.

[![NPM](https://nodei.co/npm/simplecrawler.png?downloads=true)](https://www.npmjs.com/package/simplecrawler)

[![apidoc](https://npmdoc.github.io/node-npmdoc-simplecrawler/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-simplecrawler_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-simplecrawler/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-simplecrawler/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-simplecrawler/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Christopher Giffard",
        "email": "christopher.giffard@cgiffard.com"
    },
    "bin": {
        "crawl": "./lib/cli.js"
    },
    "bugs": {
        "url": "https://github.com/cgiffard/node-simplecrawler/issues"
    },
    "dependencies": {
        "async": "^2.1.4",
        "iconv-lite": "^0.4.13",
        "robots-parser": "^1.0.0",
        "urijs": "^1.16.1"
    },
    "description": "Very straightforward, event driven web crawler. Features a flexible queue interface and a basic cache mechanism with extensible backend.",
    "devDependencies": {
        "chai": "^3.2.0",
        "eslint": "^2.0.0",
        "jsdoc": "^3.4.0",
        "mocha": "^3.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "5893d24d25ca67ca1244d813ff56ca04fadbdbe9",
        "tarball": "https://registry.npmjs.org/simplecrawler/-/simplecrawler-1.1.1.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "files": [
        "lib"
    ],
    "gitHead": "28aee5dc5d9123efb6ab4314cea4d0b7a3a25b59",
    "homepage": "https://github.com/cgiffard/node-simplecrawler",
    "keywords": [
        "simple",
        "crawler",
        "spider",
        "cache",
        "queue",
        "simplecrawler",
        "eventemitter"
    ],
    "license": "BSD-2-Clause",
    "main": "./lib/index.js",
    "maintainers": [
        {
            "name": "cgiffard",
            "email": "christopher.giffard@cgiffard.com"
        },
        {
            "name": "fredrikekelund",
            "email": "fredrik@fredrik.computer"
        }
    ],
    "name": "simplecrawler",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/cgiffard/node-simplecrawler.git"
    },
    "scripts": {
        "docs": "jsdoc -c jsdoc.json",
        "lint": "eslint example/ lib/ test/",
        "mocha": "mocha -R spec -t 5000",
        "test": "npm run lint && npm run mocha"
    },
    "version": "1.1.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module simplecrawler](#apidoc.module.simplecrawler)
1.  [function <span class="apidocSignatureSpan">simplecrawler.</span>cache (cacheLoadParameter, cacheBackend)](#apidoc.element.simplecrawler.cache)
1.  [function <span class="apidocSignatureSpan">simplecrawler.</span>cookies ()](#apidoc.element.simplecrawler.cookies)
1.  [function <span class="apidocSignatureSpan">simplecrawler.</span>crawl ()](#apidoc.element.simplecrawler.crawl)
1.  [function <span class="apidocSignatureSpan">simplecrawler.</span>queue ()](#apidoc.element.simplecrawler.queue)
1.  [function <span class="apidocSignatureSpan">simplecrawler.</span>super_ ()](#apidoc.element.simplecrawler.super_)
1.  object <span class="apidocSignatureSpan">simplecrawler.</span>cache.prototype
1.  object <span class="apidocSignatureSpan">simplecrawler.</span>cookies.prototype
1.  object <span class="apidocSignatureSpan">simplecrawler.</span>queue.prototype

#### [module simplecrawler.cache](#apidoc.module.simplecrawler.cache)
1.  [function <span class="apidocSignatureSpan">simplecrawler.</span>cache (cacheLoadParameter, cacheBackend)](#apidoc.element.simplecrawler.cache.cache)
1.  [function <span class="apidocSignatureSpan">simplecrawler.cache.</span>Cache (cacheLoadParameter, cacheBackend)](#apidoc.element.simplecrawler.cache.Cache)
1.  [function <span class="apidocSignatureSpan">simplecrawler.cache.</span>FilesystemBackend (loadParameter)](#apidoc.element.simplecrawler.cache.FilesystemBackend)

#### [module simplecrawler.cache.prototype](#apidoc.module.simplecrawler.cache.prototype)
1.  [function <span class="apidocSignatureSpan">simplecrawler.cache.prototype.</span>getCacheData (queueObject, callback)](#apidoc.element.simplecrawler.cache.prototype.getCacheData)
1.  [function <span class="apidocSignatureSpan">simplecrawler.cache.prototype.</span>saveCache ()](#apidoc.element.simplecrawler.cache.prototype.saveCache)
1.  [function <span class="apidocSignatureSpan">simplecrawler.cache.prototype.</span>setCacheData (queueObject, data, callback)](#apidoc.element.simplecrawler.cache.prototype.setCacheData)
1.  number <span class="apidocSignatureSpan">simplecrawler.cache.prototype.</span>_eventsCount
1.  object <span class="apidocSignatureSpan">simplecrawler.cache.prototype.</span>_events
1.  object <span class="apidocSignatureSpan">simplecrawler.cache.prototype.</span>domain

#### [module simplecrawler.cookies](#apidoc.module.simplecrawler.cookies)
1.  [function <span class="apidocSignatureSpan">simplecrawler.</span>cookies ()](#apidoc.element.simplecrawler.cookies.cookies)
1.  [function <span class="apidocSignatureSpan">simplecrawler.cookies.</span>Cookie (name, value, expires, path, domain, httponly)](#apidoc.element.simplecrawler.cookies.Cookie)
1.  [function <span class="apidocSignatureSpan">simplecrawler.cookies.</span>super_ ()](#apidoc.element.simplecrawler.cookies.super_)

#### [module simplecrawler.cookies.prototype](#apidoc.module.simplecrawler.cookies.prototype)
1.  [function <span class="apidocSignatureSpan">simplecrawler.cookies.prototype.</span>add (name, value, expiry, path, domain, httponly, callback)](#apidoc.element.simplecrawler.cookies.prototype.add)
1.  [function <span class="apidocSignatureSpan">simplecrawler.cookies.prototype.</span>addFromHeaders (headers, callback)](#apidoc.element.simplecrawler.cookies.prototype.addFromHeaders)
1.  [function <span class="apidocSignatureSpan">simplecrawler.cookies.prototype.</span>get (name, domain, callback)](#apidoc.element.simplecrawler.cookies.prototype.get)
1.  [function <span class="apidocSignatureSpan">simplecrawler.cookies.prototype.</span>getAsHeader (domain, path, callback)](#apidoc.element.simplecrawler.cookies.prototype.getAsHeader)
1.  [function <span class="apidocSignatureSpan">simplecrawler.cookies.prototype.</span>remove (name, domain, callback)](#apidoc.element.simplecrawler.cookies.prototype.remove)
1.  [function <span class="apidocSignatureSpan">simplecrawler.cookies.prototype.</span>toString ()](#apidoc.element.simplecrawler.cookies.prototype.toString)

#### [module simplecrawler.queue](#apidoc.module.simplecrawler.queue)
1.  [function <span class="apidocSignatureSpan">simplecrawler.</span>queue ()](#apidoc.element.simplecrawler.queue.queue)
1.  [function <span class="apidocSignatureSpan">simplecrawler.queue.</span>super_ ()](#apidoc.element.simplecrawler.queue.super_)

#### [module simplecrawler.queue.prototype](#apidoc.module.simplecrawler.queue.prototype)
1.  [function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>add (queueItem, force, callback)](#apidoc.element.simplecrawler.queue.prototype.add)
1.  [function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>avg (statisticName, callback)](#apidoc.element.simplecrawler.queue.prototype.avg)
1.  [function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>countItems (comparator, callback)](#apidoc.element.simplecrawler.queue.prototype.countItems)
1.  [function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>defrost (filename, callback)](#apidoc.element.simplecrawler.queue.prototype.defrost)
1.  [function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>exists (url, callback)](#apidoc.element.simplecrawler.queue.prototype.exists)
1.  [function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>filterItems (comparator, callback)](#apidoc.element.simplecrawler.queue.prototype.filterItems)
1.  [function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>freeze (filename, callback)](#apidoc.element.simplecrawler.queue.prototype.freeze)
1.  [function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>get (index, callback)](#apidoc.element.simplecrawler.queue.prototype.get)
1.  [function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>getLength (callback)](#apidoc.element.simplecrawler.queue.prototype.getLength)
1.  [function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>max (statisticName, callback)](#apidoc.element.simplecrawler.queue.prototype.max)
1.  [function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>min (statisticName, callback)](#apidoc.element.simplecrawler.queue.prototype.min)
1.  [function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>oldestUnfetchedItem (callback)](#apidoc.element.simplecrawler.queue.prototype.oldestUnfetchedItem)
1.  [function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>update (id, updates, callback)](#apidoc.element.simplecrawler.queue.prototype.update)



# <a name="apidoc.module.simplecrawler"></a>[module simplecrawler](#apidoc.module.simplecrawler)

#### <a name="apidoc.element.simplecrawler.cache"></a>[function <span class="apidocSignatureSpan">simplecrawler.</span>cache (cacheLoadParameter, cacheBackend)](#apidoc.element.simplecrawler.cache)
- description and source-code
```javascript
function Cache(cacheLoadParameter, cacheBackend) {

    // Ensure parameters are how we want them...
    cacheBackend = typeof cacheBackend === "object" ? cacheBackend : FilesystemBackend;
    cacheLoadParameter = cacheLoadParameter instanceof Array ? cacheLoadParameter : [cacheLoadParameter];

    // Now we can just run the factory.
    this.datastore = cacheBackend.apply(cacheBackend, cacheLoadParameter);

    // Instruct the backend to load up.
    this.datastore.load();
}
```
- example usage
```shell
...
    default 'discoverResources' function is used.*
* 'crawler.cache' -
    Specify a cache architecture to use when crawling. Must implement
    'SimpleCache' interface. You can save the site to disk using the built in
    file system cache like this:

    '''js
    crawler.cache = new Crawler.cache('pathToCacheDirectory');
    '''

* 'crawler.useProxy=false' -
    The crawler should use an HTTP proxy to make its requests.
* 'crawler.proxyHostname="127.0.0.1"' -
    The hostname of the proxy to use for requests.
* 'crawler.proxyPort=8123' -
...
```

#### <a name="apidoc.element.simplecrawler.cookies"></a>[function <span class="apidocSignatureSpan">simplecrawler.</span>cookies ()](#apidoc.element.simplecrawler.cookies)
- description and source-code
```javascript
cookies = function () {
    EventEmitter.call(this);

<span class="apidocCodeCommentSpan">    /**
     * The actual jar that holds the cookies
     * @private
     * @type {Array}
     */
</span>    this.cookies = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.simplecrawler.crawl"></a>[function <span class="apidocSignatureSpan">simplecrawler.</span>crawl ()](#apidoc.element.simplecrawler.crawl)
- description and source-code
```javascript
crawl = function () {
    throw new Error(
        "Crawler.crawl is deprecated as of version 1.0.0! " +
        "You can now pass a single URL directly to the constructor. " +
        "See the documentation for more details!"
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.simplecrawler.queue"></a>[function <span class="apidocSignatureSpan">simplecrawler.</span>queue ()](#apidoc.element.simplecrawler.queue)
- description and source-code
```javascript
queue = function () {
    Array.call(this);

<span class="apidocCodeCommentSpan">    /**
     * Speeds up {@link FetchQueue.oldestUnfetchedItem} by storing the index at
     * which the latest oldest unfetched queue item was found.
     * @name FetchQueue._oldestUnfetchedIndex
     * @private
     * @type {Number}
     */
</span>    Object.defineProperty(this, "_oldestUnfetchedIndex", {
        enumerable: false,
        writable: true,
        value: 0
    });

    /**
     * Serves as a cache for what URL's have been fetched. Keys are URL's,
     * values are booleans.
     * @name FetchQueue._scanIndex
     * @private
     * @type {Object}
     */
    Object.defineProperty(this, "_scanIndex", {
        enumerable: false,
        writable: true,
        value: {}
    });

    /**
     * Controls what properties can be operated on with the
     * {@link FetchQueue#min}, {@link FetchQueue#avg} and {@link FetchQueue#max}
     * methods.
     * @name FetchQueue._allowedStatistics
     * @type {Array}
     */
    Object.defineProperty(this, "_allowedStatistics", {
        enumerable: false,
        writable: true,
        value: [
            "actualDataSize",
            "contentLength",
            "downloadTime",
            "requestLatency",
            "requestTime"
        ]
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.simplecrawler.super_"></a>[function <span class="apidocSignatureSpan">simplecrawler.</span>super_ ()](#apidoc.element.simplecrawler.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.simplecrawler.cache"></a>[module simplecrawler.cache](#apidoc.module.simplecrawler.cache)

#### <a name="apidoc.element.simplecrawler.cache.cache"></a>[function <span class="apidocSignatureSpan">simplecrawler.</span>cache (cacheLoadParameter, cacheBackend)](#apidoc.element.simplecrawler.cache.cache)
- description and source-code
```javascript
function Cache(cacheLoadParameter, cacheBackend) {

    // Ensure parameters are how we want them...
    cacheBackend = typeof cacheBackend === "object" ? cacheBackend : FilesystemBackend;
    cacheLoadParameter = cacheLoadParameter instanceof Array ? cacheLoadParameter : [cacheLoadParameter];

    // Now we can just run the factory.
    this.datastore = cacheBackend.apply(cacheBackend, cacheLoadParameter);

    // Instruct the backend to load up.
    this.datastore.load();
}
```
- example usage
```shell
...
    default 'discoverResources' function is used.*
* 'crawler.cache' -
    Specify a cache architecture to use when crawling. Must implement
    'SimpleCache' interface. You can save the site to disk using the built in
    file system cache like this:

    '''js
    crawler.cache = new Crawler.cache('pathToCacheDirectory');
    '''

* 'crawler.useProxy=false' -
    The crawler should use an HTTP proxy to make its requests.
* 'crawler.proxyHostname="127.0.0.1"' -
    The hostname of the proxy to use for requests.
* 'crawler.proxyPort=8123' -
...
```

#### <a name="apidoc.element.simplecrawler.cache.Cache"></a>[function <span class="apidocSignatureSpan">simplecrawler.cache.</span>Cache (cacheLoadParameter, cacheBackend)](#apidoc.element.simplecrawler.cache.Cache)
- description and source-code
```javascript
function Cache(cacheLoadParameter, cacheBackend) {

    // Ensure parameters are how we want them...
    cacheBackend = typeof cacheBackend === "object" ? cacheBackend : FilesystemBackend;
    cacheLoadParameter = cacheLoadParameter instanceof Array ? cacheLoadParameter : [cacheLoadParameter];

    // Now we can just run the factory.
    this.datastore = cacheBackend.apply(cacheBackend, cacheLoadParameter);

    // Instruct the backend to load up.
    this.datastore.load();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.simplecrawler.cache.FilesystemBackend"></a>[function <span class="apidocSignatureSpan">simplecrawler.cache.</span>FilesystemBackend (loadParameter)](#apidoc.element.simplecrawler.cache.FilesystemBackend)
- description and source-code
```javascript
function backend(loadParameter) {
    return new FSBackend(loadParameter);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.simplecrawler.cache.prototype"></a>[module simplecrawler.cache.prototype](#apidoc.module.simplecrawler.cache.prototype)

#### <a name="apidoc.element.simplecrawler.cache.prototype.getCacheData"></a>[function <span class="apidocSignatureSpan">simplecrawler.cache.prototype.</span>getCacheData (queueObject, callback)](#apidoc.element.simplecrawler.cache.prototype.getCacheData)
- description and source-code
```javascript
getCacheData = function (queueObject, callback) {
    this.datastore.getItem(queueObject, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.simplecrawler.cache.prototype.saveCache"></a>[function <span class="apidocSignatureSpan">simplecrawler.cache.prototype.</span>saveCache ()](#apidoc.element.simplecrawler.cache.prototype.saveCache)
- description and source-code
```javascript
saveCache = function () {
    this.datastore.saveCache();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.simplecrawler.cache.prototype.setCacheData"></a>[function <span class="apidocSignatureSpan">simplecrawler.cache.prototype.</span>setCacheData (queueObject, data, callback)](#apidoc.element.simplecrawler.cache.prototype.setCacheData)
- description and source-code
```javascript
setCacheData = function (queueObject, data, callback) {
    this.datastore.setItem(queueObject, data, callback);
    this.emit("setcache", queueObject, data);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.simplecrawler.cookies"></a>[module simplecrawler.cookies](#apidoc.module.simplecrawler.cookies)

#### <a name="apidoc.element.simplecrawler.cookies.cookies"></a>[function <span class="apidocSignatureSpan">simplecrawler.</span>cookies ()](#apidoc.element.simplecrawler.cookies.cookies)
- description and source-code
```javascript
cookies = function () {
    EventEmitter.call(this);

<span class="apidocCodeCommentSpan">    /**
     * The actual jar that holds the cookies
     * @private
     * @type {Array}
     */
</span>    this.cookies = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.simplecrawler.cookies.Cookie"></a>[function <span class="apidocSignatureSpan">simplecrawler.cookies.</span>Cookie (name, value, expires, path, domain, httponly)](#apidoc.element.simplecrawler.cookies.Cookie)
- description and source-code
```javascript
Cookie = function (name, value, expires, path, domain, httponly) {
    if (!name) {
        throw new Error("A name is required to create a cookie.");
    }

    // Parse date to timestamp - consider it never expiring if timestamp is not
    // passed to the function
    if (expires) {

        if (typeof expires !== "number") {
            expires = (new Date(expires)).getTime();
        }

    } else {
        expires = -1;
    }

    this.name = name;
    this.value = value || "";
    this.expires = expires;
    this.path = path || "/";
    this.domain = domain || "*";
    this.httponly = Boolean(httponly);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.simplecrawler.cookies.super_"></a>[function <span class="apidocSignatureSpan">simplecrawler.cookies.</span>super_ ()](#apidoc.element.simplecrawler.cookies.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.simplecrawler.cookies.prototype"></a>[module simplecrawler.cookies.prototype](#apidoc.module.simplecrawler.cookies.prototype)

#### <a name="apidoc.element.simplecrawler.cookies.prototype.add"></a>[function <span class="apidocSignatureSpan">simplecrawler.cookies.prototype.</span>add (name, value, expiry, path, domain, httponly, callback)](#apidoc.element.simplecrawler.cookies.prototype.add)
- description and source-code
```javascript
add = function (name, value, expiry, path, domain, httponly, callback) {
    var existingIndex = -1, newCookie;

    if (arguments.length > 1) {
        newCookie = new Cookie(name, value, expiry, path, domain, httponly);
    } else if (name instanceof Cookie) {
        newCookie = name;
    } else {
        newCookie = Cookie.fromString(name);
    }

    // Are we updating an existing cookie or adding a new one?
    this.cookies.forEach(function(cookie, index) {
        if (cookie.name === newCookie.name && cookie.matchDomain(newCookie.domain)) {
            existingIndex = index;
        }
    });

    if (existingIndex === -1) {
        this.cookies.push(newCookie);
    } else {
        this.cookies[existingIndex] = newCookie;
    }

<span class="apidocCodeCommentSpan">    /**
     * Fired when a cookie has been added to the jar
     * @event CookieJar#addcookie
     * @param {Cookie} cookie The cookie that has been added
     */
</span>    this.emit("addcookie", newCookie);

    if (callback instanceof Function) {
        callback(null, newCookie);
    }

    return this;
}
```
- example usage
```shell
...
var jar = this;

if (!Array.isArray(headers)) {
    headers = [headers];
}

headers.forEach(function(header) {
    jar.add(header);
});

if (callback instanceof Function) {
    callback(null);
}

return jar;
...
```

#### <a name="apidoc.element.simplecrawler.cookies.prototype.addFromHeaders"></a>[function <span class="apidocSignatureSpan">simplecrawler.cookies.prototype.</span>addFromHeaders (headers, callback)](#apidoc.element.simplecrawler.cookies.prototype.addFromHeaders)
- description and source-code
```javascript
addFromHeaders = function (headers, callback) {
    var jar = this;

    if (!Array.isArray(headers)) {
        headers = [headers];
    }

    headers.forEach(function(header) {
        jar.add(header);
    });

    if (callback instanceof Function) {
        callback(null);
    }

    return jar;
}
```
- example usage
```shell
...
// request and the next
jar: true
    }, function (error, response, body) {
// Start by saving the cookies. We'll likely be assigned a session cookie
// straight off the bat, and then the server will remember the fact that
// this session is logged in as user "iamauser" after we've successfully
// logged in
crawler.cookies.addFromHeaders(response.headers["set-cookie"]);

// We want to get the names and values of all relevant inputs on the page,
// so that any CSRF tokens or similar things are included in the POST
// request
var $ = cheerio.load(body),
    formDefaults = {},
    // You should adapt these selectors so that they target the
...
```

#### <a name="apidoc.element.simplecrawler.cookies.prototype.get"></a>[function <span class="apidocSignatureSpan">simplecrawler.cookies.prototype.</span>get (name, domain, callback)](#apidoc.element.simplecrawler.cookies.prototype.get)
- description and source-code
```javascript
get = function (name, domain, callback) {
    var cookies = this.cookies.filter(function(cookie) {
        // If the names don't match, we're not returning this cookie
        if (Boolean(name) && cookie.name !== name) {
            return false;
        }

        // If the domains don't match, we're not returning this cookie
        if (Boolean(domain) && !cookie.matchDomain(domain)) {
            return false;
        }

        return true;
    });

    if (callback instanceof Function) {
        callback(null, cookies);
    }

    return cookies;
}
```
- example usage
```shell
...
Like any other web crawler, simplecrawler has a queue. It can be directly
accessed through 'crawler.queue' and implements an asynchronous interface for
accessing queue items and statistics. There are several methods for interacting
with the queue, the simplest being 'crawler.queue.get', which lets you get a
queue item at a specific index in the queue.

'''js
crawler.queue.get(5, function (queueItem) {
    // Do something with the queueItem
});
'''

*All queue method are in reality synchronous by default, but simplecrawler is
built to be able to use different queues that implement the same interface, and
those implementations can be asynchronous - which means they could eg. be backed
...
```

#### <a name="apidoc.element.simplecrawler.cookies.prototype.getAsHeader"></a>[function <span class="apidocSignatureSpan">simplecrawler.cookies.prototype.</span>getAsHeader (domain, path, callback)](#apidoc.element.simplecrawler.cookies.prototype.getAsHeader)
- description and source-code
```javascript
getAsHeader = function (domain, path, callback) {
    var headers = this.cookies.filter(function(cookie) {
        if (cookie.isExpired()) {
            return false;
        }
        if (!domain && !path) {
            return true;
        }
        if (domain) {
            return cookie.matchDomain(domain);
        }
        if (path) {
            return cookie.matchPath(path);
        }
    })
    .map(function(cookie) {
        return cookie.toString();
    });

    if (callback instanceof Function) {
        callback(null, headers);
    }

    return headers;
}
```
- example usage
```shell
...
};

/**
* Generates a newline-separated list of all cookies in the jar
* @return {String} Returns stringified versions of all cookies in the jar in a newline separated string
*/
CookieJar.prototype.toString = function() {
   return this.getAsHeader().join("\n");
};


/**
* Creates a new cookies
* @class
* @param {String} name                       Name of the new cookie
...
```

#### <a name="apidoc.element.simplecrawler.cookies.prototype.remove"></a>[function <span class="apidocSignatureSpan">simplecrawler.cookies.prototype.</span>remove (name, domain, callback)](#apidoc.element.simplecrawler.cookies.prototype.remove)
- description and source-code
```javascript
remove = function (name, domain, callback) {
    var cookiesRemoved = [],
        jar = this;

    jar.cookies.forEach(function(cookie, index) {
        // If the names don't match, we're not removing this cookie
        if (Boolean(name) && cookie.name !== name) {
            return false;
        }

        // If the domains don't match, we're not removing this cookie
        if (Boolean(domain) && !cookie.matchDomain(domain)) {
            return false;
        }

        // Matched. Remove!
        cookiesRemoved.push(jar.cookies.splice(index, 1));
    });

<span class="apidocCodeCommentSpan">    /**
     * Fired when one or multiple cookie have been removed from the jar
     * @event CookieJar#removecookie
     * @param {Cookie[]} cookie The cookies that have been removed
     */
</span>    jar.emit("removecookie", cookiesRemoved);

    if (callback instanceof Function) {
        callback(null, cookiesRemoved);
    }

    return cookiesRemoved;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.simplecrawler.cookies.prototype.toString"></a>[function <span class="apidocSignatureSpan">simplecrawler.cookies.prototype.</span>toString ()](#apidoc.element.simplecrawler.cookies.prototype.toString)
- description and source-code
```javascript
toString = function () {
    return this.getAsHeader().join("\n");
}
```
- example usage
```shell
...
browser, like phantomJS.

The example below demonstrates how one might achieve basic HTML-correct
discovery of only link tags using cheerio.

'''js
crawler.discoverResources = function(buffer, queueItem) {
    var $ = cheerio.load(buffer.toString("utf8"));

    return $("a[href]").map(function () {
        return $(this).attr("href");
    }).get();
};
'''
...
```



# <a name="apidoc.module.simplecrawler.queue"></a>[module simplecrawler.queue](#apidoc.module.simplecrawler.queue)

#### <a name="apidoc.element.simplecrawler.queue.queue"></a>[function <span class="apidocSignatureSpan">simplecrawler.</span>queue ()](#apidoc.element.simplecrawler.queue.queue)
- description and source-code
```javascript
queue = function () {
    Array.call(this);

<span class="apidocCodeCommentSpan">    /**
     * Speeds up {@link FetchQueue.oldestUnfetchedItem} by storing the index at
     * which the latest oldest unfetched queue item was found.
     * @name FetchQueue._oldestUnfetchedIndex
     * @private
     * @type {Number}
     */
</span>    Object.defineProperty(this, "_oldestUnfetchedIndex", {
        enumerable: false,
        writable: true,
        value: 0
    });

    /**
     * Serves as a cache for what URL's have been fetched. Keys are URL's,
     * values are booleans.
     * @name FetchQueue._scanIndex
     * @private
     * @type {Object}
     */
    Object.defineProperty(this, "_scanIndex", {
        enumerable: false,
        writable: true,
        value: {}
    });

    /**
     * Controls what properties can be operated on with the
     * {@link FetchQueue#min}, {@link FetchQueue#avg} and {@link FetchQueue#max}
     * methods.
     * @name FetchQueue._allowedStatistics
     * @type {Array}
     */
    Object.defineProperty(this, "_allowedStatistics", {
        enumerable: false,
        writable: true,
        value: [
            "actualDataSize",
            "contentLength",
            "downloadTime",
            "requestLatency",
            "requestTime"
        ]
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.simplecrawler.queue.super_"></a>[function <span class="apidocSignatureSpan">simplecrawler.queue.</span>super_ ()](#apidoc.element.simplecrawler.queue.super_)
- description and source-code
```javascript
function Array() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.simplecrawler.queue.prototype"></a>[module simplecrawler.queue.prototype](#apidoc.module.simplecrawler.queue.prototype)

#### <a name="apidoc.element.simplecrawler.queue.prototype.add"></a>[function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>add (queueItem, force, callback)](#apidoc.element.simplecrawler.queue.prototype.add)
- description and source-code
```javascript
add = function (queueItem, force, callback) {
    var queue = this;

    function addToQueue() {
        queue._scanIndex[queueItem.url] = true;
        queueItem.id = queue.length;
        queueItem.status = "queued";
        queue.push(queueItem);
        callback(null, queueItem);
    }

    queue.exists(queueItem.url, function(err, exists) {
        if (err) {
            callback(err);
        } else if (!exists) {
            addToQueue();
        } else if (force) {
            if (queue.indexOf(queueItem) > -1) {
                callback(new Error("Can't add a queueItem instance twice. You may create a new one from the same URL however."));
            } else {
                addToQueue();
            }
        } else {
            var error = new Error("Resource already exists in queue!");
            error.code = "DUPLICATE";
            callback(error);
        }
    });
}
```
- example usage
```shell
...
var jar = this;

if (!Array.isArray(headers)) {
    headers = [headers];
}

headers.forEach(function(header) {
    jar.add(header);
});

if (callback instanceof Function) {
    callback(null);
}

return jar;
...
```

#### <a name="apidoc.element.simplecrawler.queue.prototype.avg"></a>[function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>avg (statisticName, callback)](#apidoc.element.simplecrawler.queue.prototype.avg)
- description and source-code
```javascript
avg = function (statisticName, callback) {
    var sum = 0,
        count = 0,
        queue = this;

    if (queue._allowedStatistics.indexOf(statisticName) === -1) {
        return callback(new Error("Invalid statistic"));
    }

    queue.forEach(function(item) {
        if (item.fetched && Number.isFinite(item.stateData[statisticName])) {
            sum += item.stateData[statisticName];
            count++;
        }
    });

    callback(null, sum / count);
}
```
- example usage
```shell
...
'''js
crawler.queue.max("requestLatency", function(error, max) {
    console.log("The maximum request latency was %dms.", max);
});
crawler.queue.min("downloadTime", function(error, min) {
    console.log("The minimum download time was %dms.", min);
});
crawler.queue.avg("actualDataSize", function(error, avg) {
    console.log("The average resource size received is %d bytes.", avg);
});
'''

For general filtering or counting of queue items, there are two methods:
'crawler.queue.filterItems' and 'crawler.queue.countItems'. Both take an object
comparator and a callback.
...
```

#### <a name="apidoc.element.simplecrawler.queue.prototype.countItems"></a>[function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>countItems (comparator, callback)](#apidoc.element.simplecrawler.queue.prototype.countItems)
- description and source-code
```javascript
countItems = function (comparator, callback) {
    this.filterItems(comparator, function(error, items) {
        if (error) {
            callback(error);
        } else {
            callback(null, items.length);
        }
    });
}
```
- example usage
```shell
...
'''

For general filtering or counting of queue items, there are two methods:
'crawler.queue.filterItems' and 'crawler.queue.countItems'. Both take an object
comparator and a callback.

'''js
crawler.queue.countItems({ fetched: true }, function(error, count) {
    console.log("The number of completed items is %d", count);
});

crawler.queue.filterItems({ status: "notfound" }, function(error, items) {
    console.log("These items returned 404 or 410 HTTP statuses", items);
});
'''
...
```

#### <a name="apidoc.element.simplecrawler.queue.prototype.defrost"></a>[function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>defrost (filename, callback)](#apidoc.element.simplecrawler.queue.prototype.defrost)
- description and source-code
```javascript
defrost = function (filename, callback) {
    var queue = this,
        defrostedQueue = [];

    fs.readFile(filename, function(err, fileData) {
        if (err) {
            return callback(err);
        }

        if (!fileData.toString("utf8").length) {
            return callback(new Error("Failed to defrost queue from zero-length JSON."));
        }

        try {
            defrostedQueue = JSON.parse(fileData.toString("utf8"));
        } catch (error) {
            return callback(error);
        }

        queue._oldestUnfetchedIndex = defrostedQueue.length - 1;
        queue._scanIndex = {};

        for (var i = 0; i < defrostedQueue.length; i++) {
            var queueItem = defrostedQueue[i];
            queue.push(queueItem);

            if (queueItem.status === "queued") {
                queue._oldestUnfetchedIndex = Math.min(queue._oldestUnfetchedIndex, i);
            }

            queue._scanIndex[queueItem.url] = true;
        }

        callback(null, queue);
    });
}
```
- example usage
```shell
...
otherwise you'll get an empty file.

'''js
crawler.queue.freeze("mysavedqueue.json", function () {
    process.exit();
});

crawler.queue.defrost("mysavedqueue.json");
'''

## Cookies

simplecrawler has an internal cookie jar, which collects and resends cookies
automatically and by default. If you want to turn this off, set the
'crawler.acceptCookies' option to 'false'. The cookie jar is accessible via
...
```

#### <a name="apidoc.element.simplecrawler.queue.prototype.exists"></a>[function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>exists (url, callback)](#apidoc.element.simplecrawler.queue.prototype.exists)
- description and source-code
```javascript
exists = function (url, callback) {
    if (this._scanIndex[url]) {
        callback(null, 1);
    } else {
        callback(null, 0);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.simplecrawler.queue.prototype.filterItems"></a>[function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>filterItems (comparator, callback)](#apidoc.element.simplecrawler.queue.prototype.filterItems)
- description and source-code
```javascript
filterItems = function (comparator, callback) {
    var items = this.filter(function(queueItem) {
        return compare(comparator, queueItem);
    });

    callback(null, items);
}
```
- example usage
```shell
...
comparator and a callback.

'''js
crawler.queue.countItems({ fetched: true }, function(error, count) {
    console.log("The number of completed items is %d", count);
});

crawler.queue.filterItems({ status: "notfound" }, function(error, items) {
    console.log("These items returned 404 or 410 HTTP statuses", items);
});
'''

The object comparator can also contain other objects, so you may filter queue
items based on properties in their 'stateData' object as well.
...
```

#### <a name="apidoc.element.simplecrawler.queue.prototype.freeze"></a>[function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>freeze (filename, callback)](#apidoc.element.simplecrawler.queue.prototype.freeze)
- description and source-code
```javascript
freeze = function (filename, callback) {
    var queue = this;

    // Re-queue in-progress items before freezing...
    queue.forEach(function(item) {
        if (item.fetched !== true) {
            item.status = "queued";
        }
    });

    fs.writeFile(filename, JSON.stringify(queue, null, 2), function(err) {
        callback(err);
    });
}
```
- example usage
```shell
...
commences and stops is perfectly reasonable.

Note that the methods themselves are asynchronous, so if you are going to exit
the process after you do the freezing, make sure you wait for callback -
otherwise you'll get an empty file.

'''js
crawler.queue.freeze("mysavedqueue.json", function () {
    process.exit();
});

crawler.queue.defrost("mysavedqueue.json");
'''

## Cookies
...
```

#### <a name="apidoc.element.simplecrawler.queue.prototype.get"></a>[function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>get (index, callback)](#apidoc.element.simplecrawler.queue.prototype.get)
- description and source-code
```javascript
get = function (index, callback) {
    var queue = this;

    queue.getLength(function(error, length) {
        if (error) {
            callback(error);
        } else if (index >= length) {
            callback(new RangeError("Index was greater than the queue's length"));
        } else {
            callback(null, queue[index]);
        }
    });
}
```
- example usage
```shell
...
Like any other web crawler, simplecrawler has a queue. It can be directly
accessed through 'crawler.queue' and implements an asynchronous interface for
accessing queue items and statistics. There are several methods for interacting
with the queue, the simplest being 'crawler.queue.get', which lets you get a
queue item at a specific index in the queue.

'''js
crawler.queue.get(5, function (queueItem) {
    // Do something with the queueItem
});
'''

*All queue method are in reality synchronous by default, but simplecrawler is
built to be able to use different queues that implement the same interface, and
those implementations can be asynchronous - which means they could eg. be backed
...
```

#### <a name="apidoc.element.simplecrawler.queue.prototype.getLength"></a>[function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>getLength (callback)](#apidoc.element.simplecrawler.queue.prototype.getLength)
- description and source-code
```javascript
getLength = function (callback) {
    callback(null, this.length);
}
```
- example usage
```shell
...
    var originalEmit = crawler.emit;
    crawler.emit = function(evtName, queueItem) {
        crawler.queue.countItems({ fetched: true }, function(err, completeCount) {
            if (err) {
throw err;
            }

            crawler.queue.getLength(function(err, length) {
if (err) {
    throw err;
}

console.log("fetched %d of %d — %d open requests, %d open listeners",
    completeCount,
    length,
...
```

#### <a name="apidoc.element.simplecrawler.queue.prototype.max"></a>[function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>max (statisticName, callback)](#apidoc.element.simplecrawler.queue.prototype.max)
- description and source-code
```javascript
max = function (statisticName, callback) {
    var maximum = 0,
        queue = this;

    if (queue._allowedStatistics.indexOf(statisticName) === -1) {
        return callback(new Error("Invalid statistic"));
    }

    queue.forEach(function(item) {
        if (item.fetched && item.stateData[statisticName] > maximum) {
            maximum = item.stateData[statisticName];
        }
    });

    callback(null, maximum);
}
```
- example usage
```shell
...
* 'actualDataSize'

You can get the maximum, minimum, and average values for each with the
'crawler.queue.max', 'crawler.queue.min', and 'crawler.queue.avg' functions
respectively.

'''js
crawler.queue.max("requestLatency", function(error, max) {
console.log("The maximum request latency was %dms.", max);
});
crawler.queue.min("downloadTime", function(error, min) {
console.log("The minimum download time was %dms.", min);
});
crawler.queue.avg("actualDataSize", function(error, avg) {
console.log("The average resource size received is %d bytes.", avg);
...
```

#### <a name="apidoc.element.simplecrawler.queue.prototype.min"></a>[function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>min (statisticName, callback)](#apidoc.element.simplecrawler.queue.prototype.min)
- description and source-code
```javascript
min = function (statisticName, callback) {
    var minimum = Infinity,
        queue = this;

    if (queue._allowedStatistics.indexOf(statisticName) === -1) {
        return callback(new Error("Invalid statistic"));
    }

    queue.forEach(function(item) {
        if (item.fetched && item.stateData[statisticName] < minimum) {
            minimum = item.stateData[statisticName];
        }
    });

    callback(null, minimum === Infinity ? 0 : minimum);
}
```
- example usage
```shell
...
'crawler.queue.max', 'crawler.queue.min', and 'crawler.queue.avg' functions
respectively.

'''js
crawler.queue.max("requestLatency", function(error, max) {
    console.log("The maximum request latency was %dms.", max);
});
crawler.queue.min("downloadTime", function(error, min) {
    console.log("The minimum download time was %dms.", min);
});
crawler.queue.avg("actualDataSize", function(error, avg) {
    console.log("The average resource size received is %d bytes.", avg);
});
'''
...
```

#### <a name="apidoc.element.simplecrawler.queue.prototype.oldestUnfetchedItem"></a>[function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>oldestUnfetchedItem (callback)](#apidoc.element.simplecrawler.queue.prototype.oldestUnfetchedItem)
- description and source-code
```javascript
oldestUnfetchedItem = function (callback) {
    var queue = this;

    for (var i = queue._oldestUnfetchedIndex; i < queue.length; i++) {
        if (queue[i].status === "queued") {
            queue._oldestUnfetchedIndex = i;
            callback(null, queue[i]);
            return;
        }
    }

    // When no unfetched queue items remain, we previously called back with an
    // error, but since it's not really an error condition, we opted to just
    // call back with (null, null) instead
    callback(null, null);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.simplecrawler.queue.prototype.update"></a>[function <span class="apidocSignatureSpan">simplecrawler.queue.prototype.</span>update (id, updates, callback)](#apidoc.element.simplecrawler.queue.prototype.update)
- description and source-code
```javascript
update = function (id, updates, callback) {
    var queue = this,
        queueItem;

    for (var i = 0; i < queue.length; i++) {
        if (queue[i].id === id) {
            queueItem = queue[i];
            break;
        }
    }

    if (!queueItem) {
        callback(new Error("No queueItem found with that URL"));
    } else {
        deepAssign(queueItem, updates);
        callback(null, queueItem);
    }
}
```
- example usage
```shell
...
// Trim whitespace. If no path is present - assume index.html.
var sanitisedPath = path.length ? path.replace(/\s*$/ig, "") : "index.html";
var headers = queueObject.stateData.headers, sanitisedPathParts;

if (sanitisedPath.match(/\?/)) {
    sanitisedPathParts = sanitisedPath.split(/\?/g);
    var resource = sanitisedPathParts.shift();
    var hashedQS = crypto.createHash("sha1").update(sanitisedPathParts.join("?")).digest("hex");
    sanitisedPath = resource + "?" + hashedQS;
}

pathStack = sanitisedPath.split(/\//g);
pathStack = pathStack.map(function(pathChunk) {
    if (pathChunk.length >= 250) {
        return crypto.createHash("sha1").update(pathChunk).digest("hex");
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
