# api documentation for  [native-dns (v0.7.0)](http://github.com/tjfontaine/node-dns)  [![npm package](https://img.shields.io/npm/v/npmdoc-native-dns.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-native-dns) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-native-dns.svg)](https://travis-ci.org/npmdoc/node-npmdoc-native-dns)
#### Replacement for the core DNS module, includes server implementation

[![NPM](https://nodei.co/npm/native-dns.png?downloads=true)](https://www.npmjs.com/package/native-dns)

[![apidoc](https://npmdoc.github.io/node-npmdoc-native-dns/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-native-dns_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-native-dns/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-native-dns/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-native-dns/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "authors": [
        "Timothy J Fontaine <tjfontaine@gmail.com> (http://atxconsulting.com)",
        "Greg Slepak <contact@taoeffect.com> (https://twitter.com/taoeffect)",
        "Matthieu Rakotojaona"
    ],
    "bugs": {
        "url": "http://github.com/tjfontaine/node-dns/issues"
    },
    "contributors": [
        {
            "name": "Timothy J Fontaine",
            "email": "tjfontaine@gmail.com"
        }
    ],
    "dependencies": {
        "ipaddr.js": "~0.1.3",
        "native-dns-cache": "~0.0.2",
        "native-dns-packet": "~0.1.1"
    },
    "description": "Replacement for the core DNS module, includes server implementation",
    "devDependencies": {
        "nodeunit": ">= 0.7.4",
        "optimist": ""
    },
    "directories": {},
    "dist": {
        "shasum": "df418636f08fb29e8fcb7ef142c822a1588ba5b7",
        "tarball": "https://registry.npmjs.org/native-dns/-/native-dns-0.7.0.tgz"
    },
    "engines": {
        "node": ">= 0.5.0"
    },
    "gitHead": "6ce835d9625a45ea7c8e8e71e36e1ebee767969e",
    "homepage": "http://github.com/tjfontaine/node-dns",
    "keywords": [
        "dns",
        "bind",
        "native"
    ],
    "main": "dns.js",
    "maintainers": [
        {
            "name": "tjfontaine",
            "email": "tjfontaine@gmail.com"
        },
        {
            "name": "taoeffect",
            "email": "contact@taoeffect.com"
        }
    ],
    "name": "native-dns",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/tjfontaine/node-dns.git"
    },
    "scripts": {
        "test": "nodeunit test"
    },
    "version": "0.7.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module native-dns](#apidoc.module.native-dns)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>A (opts)](#apidoc.element.native-dns.A)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>AAAA (opts)](#apidoc.element.native-dns.AAAA)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>CNAME (opts)](#apidoc.element.native-dns.CNAME)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>MX (opts)](#apidoc.element.native-dns.MX)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>NAPTR (opts)](#apidoc.element.native-dns.NAPTR)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>NS (opts)](#apidoc.element.native-dns.NS)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>PTR (opts)](#apidoc.element.native-dns.PTR)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>Question (opts)](#apidoc.element.native-dns.Question)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>Request (opts)](#apidoc.element.native-dns.Request)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>SOA (opts)](#apidoc.element.native-dns.SOA)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>SRV (opts)](#apidoc.element.native-dns.SRV)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>TLSA (opts)](#apidoc.element.native-dns.TLSA)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>TXT (opts)](#apidoc.element.native-dns.TXT)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>createServer (opts)](#apidoc.element.native-dns.createServer)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>createTCPServer (opts)](#apidoc.element.native-dns.createTCPServer)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>createUDPServer (opts)](#apidoc.element.native-dns.createUDPServer)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>lookup (domain, family, callback)](#apidoc.element.native-dns.lookup)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>packet (socket)](#apidoc.element.native-dns.packet)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>resolve (domain, rrtype, ip, callback)](#apidoc.element.native-dns.resolve)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>resolve4 (domain, callback)](#apidoc.element.native-dns.resolve4)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>resolve6 (domain, callback)](#apidoc.element.native-dns.resolve6)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>resolveCname (domain, callback)](#apidoc.element.native-dns.resolveCname)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>resolveMx (domain, callback)](#apidoc.element.native-dns.resolveMx)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>resolveNs (domain, callback)](#apidoc.element.native-dns.resolveNs)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>resolveSrv (domain, callback)](#apidoc.element.native-dns.resolveSrv)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>resolveTxt (domain, callback)](#apidoc.element.native-dns.resolveTxt)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>reverse (ip, callback)](#apidoc.element.native-dns.reverse)
1.  object <span class="apidocSignatureSpan">native-dns.</span>Request.prototype
1.  object <span class="apidocSignatureSpan">native-dns.</span>client
1.  object <span class="apidocSignatureSpan">native-dns.</span>consts
1.  object <span class="apidocSignatureSpan">native-dns.</span>packet.prototype
1.  object <span class="apidocSignatureSpan">native-dns.</span>pending
1.  object <span class="apidocSignatureSpan">native-dns.</span>platform
1.  object <span class="apidocSignatureSpan">native-dns.</span>server
1.  object <span class="apidocSignatureSpan">native-dns.</span>utils
1.  string <span class="apidocSignatureSpan">native-dns.</span>BADNAME
1.  string <span class="apidocSignatureSpan">native-dns.</span>BADRESP
1.  string <span class="apidocSignatureSpan">native-dns.</span>CONNREFUSED
1.  string <span class="apidocSignatureSpan">native-dns.</span>DESTRUCTION
1.  string <span class="apidocSignatureSpan">native-dns.</span>FORMERR
1.  string <span class="apidocSignatureSpan">native-dns.</span>NODATA
1.  string <span class="apidocSignatureSpan">native-dns.</span>NOMEM
1.  string <span class="apidocSignatureSpan">native-dns.</span>NOTFOUND
1.  string <span class="apidocSignatureSpan">native-dns.</span>NOTIMP
1.  string <span class="apidocSignatureSpan">native-dns.</span>REFUSED
1.  string <span class="apidocSignatureSpan">native-dns.</span>SERVFAIL
1.  string <span class="apidocSignatureSpan">native-dns.</span>TIMEOUT

#### [module native-dns.Request](#apidoc.module.native-dns.Request)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>Request (opts)](#apidoc.element.native-dns.Request.Request)
1.  [function <span class="apidocSignatureSpan">native-dns.Request.</span>super_ ()](#apidoc.element.native-dns.Request.super_)

#### [module native-dns.Request.prototype](#apidoc.module.native-dns.Request.prototype)
1.  [function <span class="apidocSignatureSpan">native-dns.Request.prototype.</span>_send ()](#apidoc.element.native-dns.Request.prototype._send)
1.  [function <span class="apidocSignatureSpan">native-dns.Request.prototype.</span>cancel ()](#apidoc.element.native-dns.Request.prototype.cancel)
1.  [function <span class="apidocSignatureSpan">native-dns.Request.prototype.</span>done ()](#apidoc.element.native-dns.Request.prototype.done)
1.  [function <span class="apidocSignatureSpan">native-dns.Request.prototype.</span>error (err)](#apidoc.element.native-dns.Request.prototype.error)
1.  [function <span class="apidocSignatureSpan">native-dns.Request.prototype.</span>handle (err, answer, cached)](#apidoc.element.native-dns.Request.prototype.handle)
1.  [function <span class="apidocSignatureSpan">native-dns.Request.prototype.</span>handleTimeout ()](#apidoc.element.native-dns.Request.prototype.handleTimeout)
1.  [function <span class="apidocSignatureSpan">native-dns.Request.prototype.</span>send ()](#apidoc.element.native-dns.Request.prototype.send)

#### [module native-dns.client](#apidoc.module.native-dns.client)
1.  [function <span class="apidocSignatureSpan">native-dns.client.</span>Request (opts)](#apidoc.element.native-dns.client.Request)
1.  [function <span class="apidocSignatureSpan">native-dns.client.</span>Resolve (opts, cb)](#apidoc.element.native-dns.client.Resolve)
1.  [function <span class="apidocSignatureSpan">native-dns.client.</span>lookup (domain, family, callback)](#apidoc.element.native-dns.client.lookup)
1.  [function <span class="apidocSignatureSpan">native-dns.client.</span>resolve (domain, rrtype, ip, callback)](#apidoc.element.native-dns.client.resolve)
1.  [function <span class="apidocSignatureSpan">native-dns.client.</span>resolve4 (domain, callback)](#apidoc.element.native-dns.client.resolve4)
1.  [function <span class="apidocSignatureSpan">native-dns.client.</span>resolve6 (domain, callback)](#apidoc.element.native-dns.client.resolve6)
1.  [function <span class="apidocSignatureSpan">native-dns.client.</span>resolveCname (domain, callback)](#apidoc.element.native-dns.client.resolveCname)
1.  [function <span class="apidocSignatureSpan">native-dns.client.</span>resolveMx (domain, callback)](#apidoc.element.native-dns.client.resolveMx)
1.  [function <span class="apidocSignatureSpan">native-dns.client.</span>resolveNs (domain, callback)](#apidoc.element.native-dns.client.resolveNs)
1.  [function <span class="apidocSignatureSpan">native-dns.client.</span>resolveSrv (domain, callback)](#apidoc.element.native-dns.client.resolveSrv)
1.  [function <span class="apidocSignatureSpan">native-dns.client.</span>resolveTlsa (domain, callback)](#apidoc.element.native-dns.client.resolveTlsa)
1.  [function <span class="apidocSignatureSpan">native-dns.client.</span>resolveTxt (domain, callback)](#apidoc.element.native-dns.client.resolveTxt)
1.  [function <span class="apidocSignatureSpan">native-dns.client.</span>reverse (ip, callback)](#apidoc.element.native-dns.client.reverse)

#### [module native-dns.consts](#apidoc.module.native-dns.consts)
1.  [function <span class="apidocSignatureSpan">native-dns.consts.</span>nameToQtype (n)](#apidoc.element.native-dns.consts.nameToQtype)
1.  [function <span class="apidocSignatureSpan">native-dns.consts.</span>qtypeToName (t)](#apidoc.element.native-dns.consts.qtypeToName)
1.  object <span class="apidocSignatureSpan">native-dns.consts.</span>FAMILY_TO_QTYPE
1.  object <span class="apidocSignatureSpan">native-dns.consts.</span>NAME_TO_QCLASS
1.  object <span class="apidocSignatureSpan">native-dns.consts.</span>NAME_TO_QTYPE
1.  object <span class="apidocSignatureSpan">native-dns.consts.</span>NAME_TO_RCODE
1.  object <span class="apidocSignatureSpan">native-dns.consts.</span>QCLASS_TO_NAME
1.  object <span class="apidocSignatureSpan">native-dns.consts.</span>QTYPE_TO_FAMILY
1.  object <span class="apidocSignatureSpan">native-dns.consts.</span>QTYPE_TO_NAME
1.  object <span class="apidocSignatureSpan">native-dns.consts.</span>RCODE_TO_NAME
1.  string <span class="apidocSignatureSpan">native-dns.consts.</span>BADNAME
1.  string <span class="apidocSignatureSpan">native-dns.consts.</span>BADRESP
1.  string <span class="apidocSignatureSpan">native-dns.consts.</span>CONNREFUSED
1.  string <span class="apidocSignatureSpan">native-dns.consts.</span>DESTRUCTION
1.  string <span class="apidocSignatureSpan">native-dns.consts.</span>FORMERR
1.  string <span class="apidocSignatureSpan">native-dns.consts.</span>NODATA
1.  string <span class="apidocSignatureSpan">native-dns.consts.</span>NOMEM
1.  string <span class="apidocSignatureSpan">native-dns.consts.</span>NOTFOUND
1.  string <span class="apidocSignatureSpan">native-dns.consts.</span>NOTIMP
1.  string <span class="apidocSignatureSpan">native-dns.consts.</span>REFUSED
1.  string <span class="apidocSignatureSpan">native-dns.consts.</span>SERVFAIL
1.  string <span class="apidocSignatureSpan">native-dns.consts.</span>TIMEOUT

#### [module native-dns.packet](#apidoc.module.native-dns.packet)
1.  [function <span class="apidocSignatureSpan">native-dns.</span>packet (socket)](#apidoc.element.native-dns.packet.packet)
1.  [function <span class="apidocSignatureSpan">native-dns.packet.</span>parse (msg, socket)](#apidoc.element.native-dns.packet.parse)
1.  [function <span class="apidocSignatureSpan">native-dns.packet.</span>super_ ()](#apidoc.element.native-dns.packet.super_)
1.  [function <span class="apidocSignatureSpan">native-dns.packet.</span>write (buff, packet)](#apidoc.element.native-dns.packet.write)

#### [module native-dns.packet.prototype](#apidoc.module.native-dns.packet.prototype)
1.  [function <span class="apidocSignatureSpan">native-dns.packet.prototype.</span>send ()](#apidoc.element.native-dns.packet.prototype.send)

#### [module native-dns.pending](#apidoc.module.native-dns.pending)
1.  [function <span class="apidocSignatureSpan">native-dns.pending.</span>remove (request)](#apidoc.element.native-dns.pending.remove)
1.  [function <span class="apidocSignatureSpan">native-dns.pending.</span>send (request)](#apidoc.element.native-dns.pending.send)

#### [module native-dns.server](#apidoc.module.native-dns.server)
1.  [function <span class="apidocSignatureSpan">native-dns.server.</span>createServer (opts)](#apidoc.element.native-dns.server.createServer)
1.  [function <span class="apidocSignatureSpan">native-dns.server.</span>createTCPServer (opts)](#apidoc.element.native-dns.server.createTCPServer)
1.  [function <span class="apidocSignatureSpan">native-dns.server.</span>createUDPServer (opts)](#apidoc.element.native-dns.server.createUDPServer)

#### [module native-dns.utils](#apidoc.module.native-dns.utils)
1.  [function <span class="apidocSignatureSpan">native-dns.utils.</span>TCPSocket (socket)](#apidoc.element.native-dns.utils.TCPSocket)
1.  [function <span class="apidocSignatureSpan">native-dns.utils.</span>UDPSocket (socket, remote)](#apidoc.element.native-dns.utils.UDPSocket)
1.  [function <span class="apidocSignatureSpan">native-dns.utils.</span>reverseIP (ip)](#apidoc.element.native-dns.utils.reverseIP)



# <a name="apidoc.module.native-dns"></a>[module native-dns](#apidoc.module.native-dns)

#### <a name="apidoc.element.native-dns.A"></a>[function <span class="apidocSignatureSpan">native-dns.</span>A (opts)](#apidoc.element.native-dns.A)
- description and source-code
```javascript
A = function (opts) {
  var obj = {};
  opts = opts || {};
  obj.type = consts.nameToQtype(type);
  obj.class = consts.NAME_TO_QCLASS.IN;
  Object.keys(opts).forEach(function (k) {
    if (opts.hasOwnProperty(k) && ['type', 'class'].indexOf(k) == -1) {
      obj[k] = opts[k];
    }
  });
  return obj;
}
```
- example usage
```shell
...

'''javascript
var dns = require('../dns'),
server = dns.createServer();

server.on('request', function (request, response) {
//console.log(request)
response.answer.push(dns.A({
  name: request.question[0].name,
  address: '127.0.0.1',
  ttl: 600,
}));
response.answer.push(dns.A({
  name: request.question[0].name,
  address: '127.0.0.2',
...
```

#### <a name="apidoc.element.native-dns.AAAA"></a>[function <span class="apidocSignatureSpan">native-dns.</span>AAAA (opts)](#apidoc.element.native-dns.AAAA)
- description and source-code
```javascript
AAAA = function (opts) {
  var obj = {};
  opts = opts || {};
  obj.type = consts.nameToQtype(type);
  obj.class = consts.NAME_TO_QCLASS.IN;
  Object.keys(opts).forEach(function (k) {
    if (opts.hasOwnProperty(k) && ['type', 'class'].indexOf(k) == -1) {
      obj[k] = opts[k];
    }
  });
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.CNAME"></a>[function <span class="apidocSignatureSpan">native-dns.</span>CNAME (opts)](#apidoc.element.native-dns.CNAME)
- description and source-code
```javascript
CNAME = function (opts) {
  var obj = {};
  opts = opts || {};
  obj.type = consts.nameToQtype(type);
  obj.class = consts.NAME_TO_QCLASS.IN;
  Object.keys(opts).forEach(function (k) {
    if (opts.hasOwnProperty(k) && ['type', 'class'].indexOf(k) == -1) {
      obj[k] = opts[k];
    }
  });
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.MX"></a>[function <span class="apidocSignatureSpan">native-dns.</span>MX (opts)](#apidoc.element.native-dns.MX)
- description and source-code
```javascript
MX = function (opts) {
  var obj = {};
  opts = opts || {};
  obj.type = consts.nameToQtype(type);
  obj.class = consts.NAME_TO_QCLASS.IN;
  Object.keys(opts).forEach(function (k) {
    if (opts.hasOwnProperty(k) && ['type', 'class'].indexOf(k) == -1) {
      obj[k] = opts[k];
    }
  });
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.NAPTR"></a>[function <span class="apidocSignatureSpan">native-dns.</span>NAPTR (opts)](#apidoc.element.native-dns.NAPTR)
- description and source-code
```javascript
NAPTR = function (opts) {
  var obj = {};
  opts = opts || {};
  obj.type = consts.nameToQtype(type);
  obj.class = consts.NAME_TO_QCLASS.IN;
  Object.keys(opts).forEach(function (k) {
    if (opts.hasOwnProperty(k) && ['type', 'class'].indexOf(k) == -1) {
      obj[k] = opts[k];
    }
  });
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.NS"></a>[function <span class="apidocSignatureSpan">native-dns.</span>NS (opts)](#apidoc.element.native-dns.NS)
- description and source-code
```javascript
NS = function (opts) {
  var obj = {};
  opts = opts || {};
  obj.type = consts.nameToQtype(type);
  obj.class = consts.NAME_TO_QCLASS.IN;
  Object.keys(opts).forEach(function (k) {
    if (opts.hasOwnProperty(k) && ['type', 'class'].indexOf(k) == -1) {
      obj[k] = opts[k];
    }
  });
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.PTR"></a>[function <span class="apidocSignatureSpan">native-dns.</span>PTR (opts)](#apidoc.element.native-dns.PTR)
- description and source-code
```javascript
PTR = function (opts) {
  var obj = {};
  opts = opts || {};
  obj.type = consts.nameToQtype(type);
  obj.class = consts.NAME_TO_QCLASS.IN;
  Object.keys(opts).forEach(function (k) {
    if (opts.hasOwnProperty(k) && ['type', 'class'].indexOf(k) == -1) {
      obj[k] = opts[k];
    }
  });
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.Question"></a>[function <span class="apidocSignatureSpan">native-dns.</span>Question (opts)](#apidoc.element.native-dns.Question)
- description and source-code
```javascript
Question = function (opts) {
  var q = {}, qtype;

  opts = opts || {};

  q.name = opts.name;

  qtype = opts.type || consts.NAME_TO_QTYPE.A;
  if (typeof(qtype) === 'string' || qtype instanceof String)
    qtype = consts.nameToQtype(qtype.toUpperCase());

  if (!qtype || typeof(qtype) !== 'number')
    throw new Error("Question type must be defined and be valid");

  q.type = qtype;

  q.class = opts.class || consts.NAME_TO_QCLASS.IN;

  return q;
}
```
- example usage
```shell
...
Beyond matching the upstream module, native-dns also provides a method for
customizing queries.

'''javascript
var dns = require('../dns'),
  util = require('util');

var question = dns.Question({
  name: 'www.google.com',
  type: 'A',
});

var start = Date.now();

var req = dns.Request({
...
```

#### <a name="apidoc.element.native-dns.Request"></a>[function <span class="apidocSignatureSpan">native-dns.</span>Request (opts)](#apidoc.element.native-dns.Request)
- description and source-code
```javascript
Request = function (opts) {
  if (!(this instanceof Request)) return new Request(opts);

  this.question = opts.question;
  this.server = opts.server;

  if (typeof(this.server) === 'string' || this.server instanceof String)
    this.server = { address: this.server, port: 53, type: 'udp'};

  if (!this.server || !this.server.address || !net.isIP(this.server.address))
    throw new Error('Server object must be supplied with at least address');

  if (!this.server.type || ['udp', 'tcp'].indexOf(this.server.type) === -1)
    this.server.type = 'udp';

  if (!this.server.port)
    this.server.port = 53;

  this.timeout = opts.timeout || 4 * 1000;
  this.try_edns = opts.try_edns || false;

  this.fired = false;
  this.id = undefined;

  if (opts.cache || opts.cache === false) {
    this.cache = opts.cache;
  } else {
    this.cache = platform.cache;
  }
  debug('request created', this.question);
}
```
- example usage
```shell
...
var question = dns.Question({
name: 'www.google.com',
type: 'A',
});

var start = Date.now();

var req = dns.Request({
question: question,
server: { address: '8.8.8.8', port: 53, type: 'udp' },
timeout: 1000,
});

req.on('timeout', function () {
console.log('Timeout in making request');
...
```

#### <a name="apidoc.element.native-dns.SOA"></a>[function <span class="apidocSignatureSpan">native-dns.</span>SOA (opts)](#apidoc.element.native-dns.SOA)
- description and source-code
```javascript
SOA = function (opts) {
  var obj = {};
  opts = opts || {};
  obj.type = consts.nameToQtype(type);
  obj.class = consts.NAME_TO_QCLASS.IN;
  Object.keys(opts).forEach(function (k) {
    if (opts.hasOwnProperty(k) && ['type', 'class'].indexOf(k) == -1) {
      obj[k] = opts[k];
    }
  });
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.SRV"></a>[function <span class="apidocSignatureSpan">native-dns.</span>SRV (opts)](#apidoc.element.native-dns.SRV)
- description and source-code
```javascript
SRV = function (opts) {
  var obj = {};
  opts = opts || {};
  obj.type = consts.nameToQtype(type);
  obj.class = consts.NAME_TO_QCLASS.IN;
  Object.keys(opts).forEach(function (k) {
    if (opts.hasOwnProperty(k) && ['type', 'class'].indexOf(k) == -1) {
      obj[k] = opts[k];
    }
  });
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.TLSA"></a>[function <span class="apidocSignatureSpan">native-dns.</span>TLSA (opts)](#apidoc.element.native-dns.TLSA)
- description and source-code
```javascript
TLSA = function (opts) {
  var obj = {};
  opts = opts || {};
  obj.type = consts.nameToQtype(type);
  obj.class = consts.NAME_TO_QCLASS.IN;
  Object.keys(opts).forEach(function (k) {
    if (opts.hasOwnProperty(k) && ['type', 'class'].indexOf(k) == -1) {
      obj[k] = opts[k];
    }
  });
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.TXT"></a>[function <span class="apidocSignatureSpan">native-dns.</span>TXT (opts)](#apidoc.element.native-dns.TXT)
- description and source-code
```javascript
TXT = function (opts) {
  var obj = {};
  opts = opts || {};
  obj.type = consts.nameToQtype(type);
  obj.class = consts.NAME_TO_QCLASS.IN;
  Object.keys(opts).forEach(function (k) {
    if (opts.hasOwnProperty(k) && ['type', 'class'].indexOf(k) == -1) {
      obj[k] = opts[k];
    }
  });
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.createServer"></a>[function <span class="apidocSignatureSpan">native-dns.</span>createServer (opts)](#apidoc.element.native-dns.createServer)
- description and source-code
```javascript
createServer = function (opts) {
  return new UDPServer(opts || {});
}
```
- example usage
```shell
...
Server
------

There is also a rudimentary server implementation

'''javascript
var dns = require('../dns'),
server = dns.createServer();

server.on('request', function (request, response) {
//console.log(request)
response.answer.push(dns.A({
  name: request.question[0].name,
  address: '127.0.0.1',
  ttl: 600,
...
```

#### <a name="apidoc.element.native-dns.createTCPServer"></a>[function <span class="apidocSignatureSpan">native-dns.</span>createTCPServer (opts)](#apidoc.element.native-dns.createTCPServer)
- description and source-code
```javascript
createTCPServer = function (opts) {
  return new TCPServer(opts || {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.createUDPServer"></a>[function <span class="apidocSignatureSpan">native-dns.</span>createUDPServer (opts)](#apidoc.element.native-dns.createUDPServer)
- description and source-code
```javascript
createUDPServer = function (opts) {
  return exports.createServer(opts);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.lookup"></a>[function <span class="apidocSignatureSpan">native-dns.</span>lookup (domain, family, callback)](#apidoc.element.native-dns.lookup)
- description and source-code
```javascript
lookup = function (domain, family, callback) {
  var rrtype, revip, res;

  if (!callback) {
    callback = family;
    family = undefined;
  }

  if (!family) {
    family = 4;
  }

  revip = net.isIP(domain);

  if (revip === 4 || revip === 6) {
    process.nextTick(function() {
      callback(null, domain, revip);
    });
    return {};
  }

  if (!domain) {
    process.nextTick(function() {
      callback(null, null, family);
    });
    return {};
  }

  rrtype = consts.FAMILY_TO_QTYPE[family];

  var opts = {
    domain: domain,
    rrtype: rrtype
  };

  res = new Lookup(opts);

  res._cb = function(err, response) {
    var i, afamily, address, a, all;

    if (err) {
      callback(err, undefined, undefined);
      return;
    }

    all = response.answer.concat(response.additional);

    for (i = 0; i < all.length; i++) {
      a = all[i];

      if (a.type === A || a.type === AAAA) {
        afamily = consts.QTYPE_TO_FAMILY[a.type];
        address = a.address;
        break;
      }
    }

    callback(err, address, afamily);
  };

  return res;
}
```
- example usage
```shell
...
};

Request.prototype.send = function() {
  debug('request starting', this.question);
  var self = this;

  if (this.cache && this.cache.lookup) {
    this.cache.lookup(this.question, function(results) {
var packet;

if (!results) {
  self._send();
} else {
  packet = new Packet();
  packet.answer = results.slice();
...
```

#### <a name="apidoc.element.native-dns.packet"></a>[function <span class="apidocSignatureSpan">native-dns.</span>packet (socket)](#apidoc.element.native-dns.packet)
- description and source-code
```javascript
packet = function (socket) {
  NDP.call(this);
  this.address = undefined;
  this._socket = socket;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.resolve"></a>[function <span class="apidocSignatureSpan">native-dns.</span>resolve (domain, rrtype, ip, callback)](#apidoc.element.native-dns.resolve)
- description and source-code
```javascript
resolve = function (domain, rrtype, ip, callback) {
  var res;

  if (!callback) {
    callback = ip;
    ip = undefined;
  }

  if (!callback) {
    callback = rrtype;
    rrtype = undefined;
  }

  rrtype = consts.NAME_TO_QTYPE[rrtype || 'A'];

  if (rrtype === PTR) {
    return reverse(domain, callback);
  }

  var opts = {
    domain: domain,
    rrtype: rrtype,
    remote: ip,
  };

  res = new Resolve(opts);

  res._cb = function(err, response) {
    var ret = [], i, a;

    if (err) {
      callback(err, response);
      return;
    }

    for (i = 0; i < response.answer.length; i++) {
      a = response.answer[i];
      if (a.type === rrtype) {
        switch (rrtype) {
          case A:
          case AAAA:
            ret.push(a.address);
            break;
          case consts.NAME_TO_QTYPE.MX:
            ret.push({
              priority: a.priority,
              exchange: a.exchange
            });
            break;
          case TXT:
          case NS:
          case CNAME:
          case PTR:
            ret.push(a.data);
            break;
          case SRV:
            ret.push({
              priority: a.priority,
              weight: a.weight,
              port: a.port,
              name: a.target
            });
            break;
          default:
            ret.push(a);
            break;
        }
      }
    }

    if (ret.length === 0) {
      ret = undefined;
    }

    callback(err, ret);
  };

  return res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.resolve4"></a>[function <span class="apidocSignatureSpan">native-dns.</span>resolve4 (domain, callback)](#apidoc.element.native-dns.resolve4)
- description and source-code
```javascript
resolve4 = function (domain, callback) {
  return resolve(domain, 'A', function(err, results) {
    callback(err, results);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.resolve6"></a>[function <span class="apidocSignatureSpan">native-dns.</span>resolve6 (domain, callback)](#apidoc.element.native-dns.resolve6)
- description and source-code
```javascript
resolve6 = function (domain, callback) {
  return resolve(domain, 'AAAA', function(err, results) {
    callback(err, results);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.resolveCname"></a>[function <span class="apidocSignatureSpan">native-dns.</span>resolveCname (domain, callback)](#apidoc.element.native-dns.resolveCname)
- description and source-code
```javascript
resolveCname = function (domain, callback) {
  return resolve(domain, 'CNAME', function(err, results) {
    callback(err, results);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.resolveMx"></a>[function <span class="apidocSignatureSpan">native-dns.</span>resolveMx (domain, callback)](#apidoc.element.native-dns.resolveMx)
- description and source-code
```javascript
resolveMx = function (domain, callback) {
  return resolve(domain, 'MX', function(err, results) {
    callback(err, results);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.resolveNs"></a>[function <span class="apidocSignatureSpan">native-dns.</span>resolveNs (domain, callback)](#apidoc.element.native-dns.resolveNs)
- description and source-code
```javascript
resolveNs = function (domain, callback) {
  return resolve(domain, 'NS', function(err, results) {
    callback(err, results);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.resolveSrv"></a>[function <span class="apidocSignatureSpan">native-dns.</span>resolveSrv (domain, callback)](#apidoc.element.native-dns.resolveSrv)
- description and source-code
```javascript
resolveSrv = function (domain, callback) {
  return resolve(domain, 'SRV', function(err, results) {
    callback(err, results);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.resolveTxt"></a>[function <span class="apidocSignatureSpan">native-dns.</span>resolveTxt (domain, callback)](#apidoc.element.native-dns.resolveTxt)
- description and source-code
```javascript
resolveTxt = function (domain, callback) {
  return resolve(domain, 'TXT', function(err, results) {
    callback(err, results);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.reverse"></a>[function <span class="apidocSignatureSpan">native-dns.</span>reverse (ip, callback)](#apidoc.element.native-dns.reverse)
- description and source-code
```javascript
reverse = function (ip, callback) {
  var error, opts, res;

  if (!net.isIP(ip)) {
    error = new Error('getHostByAddr ENOTIMP');
    error.errno = error.code = 'ENOTIMP';
    throw error;
  }

  opts = {
    domain: utils.reverseIP(ip),
    rrtype: PTR
  };

  res = new Lookup(opts);

  res._cb = function(err, response) {
    var results = [];

    if (response) {
      response.answer.forEach(function(a) {
        if (a.type === PTR) {
          results.push(a.data);
        }
      });
    }

    if (results.length === 0) {
      results = undefined;
    }

    callback(err, results);
  };

  return res;
}
```
- example usage
```shell
...

    this._server_list.push(u);
    this._server_list.push(t);

    tries += 1;
  }

  this._server_list.reverse();
};

Resolve.prototype._popServer = function() {
  debug('resolve pop server', this._current_server, this._domain);
  this._server_list.splice(0, 1, this._current_server);
};
...
```



# <a name="apidoc.module.native-dns.Request"></a>[module native-dns.Request](#apidoc.module.native-dns.Request)

#### <a name="apidoc.element.native-dns.Request.Request"></a>[function <span class="apidocSignatureSpan">native-dns.</span>Request (opts)](#apidoc.element.native-dns.Request.Request)
- description and source-code
```javascript
Request = function (opts) {
  if (!(this instanceof Request)) return new Request(opts);

  this.question = opts.question;
  this.server = opts.server;

  if (typeof(this.server) === 'string' || this.server instanceof String)
    this.server = { address: this.server, port: 53, type: 'udp'};

  if (!this.server || !this.server.address || !net.isIP(this.server.address))
    throw new Error('Server object must be supplied with at least address');

  if (!this.server.type || ['udp', 'tcp'].indexOf(this.server.type) === -1)
    this.server.type = 'udp';

  if (!this.server.port)
    this.server.port = 53;

  this.timeout = opts.timeout || 4 * 1000;
  this.try_edns = opts.try_edns || false;

  this.fired = false;
  this.id = undefined;

  if (opts.cache || opts.cache === false) {
    this.cache = opts.cache;
  } else {
    this.cache = platform.cache;
  }
  debug('request created', this.question);
}
```
- example usage
```shell
...
var question = dns.Question({
name: 'www.google.com',
type: 'A',
});

var start = Date.now();

var req = dns.Request({
question: question,
server: { address: '8.8.8.8', port: 53, type: 'udp' },
timeout: 1000,
});

req.on('timeout', function () {
console.log('Timeout in making request');
...
```

#### <a name="apidoc.element.native-dns.Request.super_"></a>[function <span class="apidocSignatureSpan">native-dns.Request.</span>super_ ()](#apidoc.element.native-dns.Request.super_)
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



# <a name="apidoc.module.native-dns.Request.prototype"></a>[module native-dns.Request.prototype](#apidoc.module.native-dns.Request.prototype)

#### <a name="apidoc.element.native-dns.Request.prototype._send"></a>[function <span class="apidocSignatureSpan">native-dns.Request.prototype.</span>_send ()](#apidoc.element.native-dns.Request.prototype._send)
- description and source-code
```javascript
_send = function () {
  debug('request not in cache', this.question);
  var self = this;

  this.timer_ = setTimeout(function() {
    self.handleTimeout();
  }, this.timeout);

  PendingRequests.send(self);
}
```
- example usage
```shell
...
var self = this;

if (this.cache && this.cache.lookup) {
  this.cache.lookup(this.question, function(results) {
    var packet;

    if (!results) {
      self._send();
    } else {
      packet = new Packet();
      packet.answer = results.slice();
      self.handle(null, packet, true);
    }
  });
} else {
...
```

#### <a name="apidoc.element.native-dns.Request.prototype.cancel"></a>[function <span class="apidocSignatureSpan">native-dns.Request.prototype.</span>cancel ()](#apidoc.element.native-dns.Request.prototype.cancel)
- description and source-code
```javascript
cancel = function () {
  debug('request cancelled', this.id, this.question);
  this.emit('cancelled');
  this.done();
}
```
- example usage
```shell
...
  this.start();
}
};
util.inherits(Resolve, EventEmitter);

Resolve.prototype.cancel = function() {
if (this._request) {
  this._request.cancel();
}
};

Resolve.prototype._buildQuestion = function(name) {
debug('building question', name);
this.question = {
  type: this._rrtype,
...
```

#### <a name="apidoc.element.native-dns.Request.prototype.done"></a>[function <span class="apidocSignatureSpan">native-dns.Request.prototype.</span>done ()](#apidoc.element.native-dns.Request.prototype.done)
- description and source-code
```javascript
done = function () {
  debug('request finished', this.id, this.question);
  this.fired = true;
  clearTimeout(this.timer_);
  PendingRequests.remove(this);
  this.emit('end');
  this.id = undefined;
}
```
- example usage
```shell
...
  debug('request handled', this.id, this.question);

  if (!cached && this.cache && this.cache.store && answer) {
    this.cache.store(answer);
  }

  this.emit('message', err, answer);
  this.done();
}
};

Request.prototype.done = function() {
debug('request finished', this.id, this.question);
this.fired = true;
clearTimeout(this.timer_);
...
```

#### <a name="apidoc.element.native-dns.Request.prototype.error"></a>[function <span class="apidocSignatureSpan">native-dns.Request.prototype.</span>error (err)](#apidoc.element.native-dns.Request.prototype.error)
- description and source-code
```javascript
error = function (err) {
  if (!this.fired) {
    debug('request error', err, this.id, this.question);
    this.emit('error', err);
    this.done();
  }
}
```
- example usage
```shell
...
    }

    packet.question.push(req.question);
    packet.send();

    this._ref();
  } catch (e) {
    req.error(e);
  }
}
};

SocketQueue.prototype._onmessage = function(msg, remote) {
var req, packet;
...
```

#### <a name="apidoc.element.native-dns.Request.prototype.handle"></a>[function <span class="apidocSignatureSpan">native-dns.Request.prototype.</span>handle (err, answer, cached)](#apidoc.element.native-dns.Request.prototype.handle)
- description and source-code
```javascript
handle = function (err, answer, cached) {
  if (!this.fired) {
    debug('request handled', this.id, this.question);

    if (!cached && this.cache && this.cache.store && answer) {
      this.cache.store(answer);
    }

    this.emit('message', err, answer);
    this.done();
  }
}
```
- example usage
```shell
...
      var packet;

      if (!results) {
        self._send();
      } else {
        packet = new Packet();
        packet.answer = results.slice();
        self.handle(null, packet, true);
      }
    });
  } else {
    this._send();
  }
};
...
```

#### <a name="apidoc.element.native-dns.Request.prototype.handleTimeout"></a>[function <span class="apidocSignatureSpan">native-dns.Request.prototype.</span>handleTimeout ()](#apidoc.element.native-dns.Request.prototype.handleTimeout)
- description and source-code
```javascript
handleTimeout = function () {
  if (!this.fired) {
    debug('request timedout', this.id, this.question);
    this.emit('timeout');
    this.done();
  }
}
```
- example usage
```shell
...
};

Request.prototype._send = function() {
debug('request not in cache', this.question);
var self = this;

this.timer_ = setTimeout(function() {
  self.handleTimeout();
}, this.timeout);

PendingRequests.send(self);
};

Request.prototype.cancel = function() {
debug('request cancelled', this.id, this.question);
...
```

#### <a name="apidoc.element.native-dns.Request.prototype.send"></a>[function <span class="apidocSignatureSpan">native-dns.Request.prototype.</span>send ()](#apidoc.element.native-dns.Request.prototype.send)
- description and source-code
```javascript
send = function () {
  debug('request starting', this.question);
  var self = this;

  if (this.cache && this.cache.lookup) {
    this.cache.lookup(this.question, function(results) {
      var packet;

      if (!results) {
        self._send();
      } else {
        packet = new Packet();
        packet.answer = results.slice();
        self.handle(null, packet, true);
      }
    });
  } else {
    this._send();
  }
}
```
- example usage
```shell
...
});

req.on('end', function () {
 var delta = (Date.now()) - start;
 console.log('Finished processing request: ' + delta.toString() + 'ms');
});

req.send();
'''

Request creation takes an object with the following fields

* 'question' -- an instance of Question (required)
* 'server' -- defines the remote end point (required)
 - as an object it should be
...
```



# <a name="apidoc.module.native-dns.client"></a>[module native-dns.client](#apidoc.module.native-dns.client)

#### <a name="apidoc.element.native-dns.client.Request"></a>[function <span class="apidocSignatureSpan">native-dns.client.</span>Request (opts)](#apidoc.element.native-dns.client.Request)
- description and source-code
```javascript
Request = function (opts) {
  if (!(this instanceof Request)) return new Request(opts);

  this.question = opts.question;
  this.server = opts.server;

  if (typeof(this.server) === 'string' || this.server instanceof String)
    this.server = { address: this.server, port: 53, type: 'udp'};

  if (!this.server || !this.server.address || !net.isIP(this.server.address))
    throw new Error('Server object must be supplied with at least address');

  if (!this.server.type || ['udp', 'tcp'].indexOf(this.server.type) === -1)
    this.server.type = 'udp';

  if (!this.server.port)
    this.server.port = 53;

  this.timeout = opts.timeout || 4 * 1000;
  this.try_edns = opts.try_edns || false;

  this.fired = false;
  this.id = undefined;

  if (opts.cache || opts.cache === false) {
    this.cache = opts.cache;
  } else {
    this.cache = platform.cache;
  }
  debug('request created', this.question);
}
```
- example usage
```shell
...
var question = dns.Question({
name: 'www.google.com',
type: 'A',
});

var start = Date.now();

var req = dns.Request({
question: question,
server: { address: '8.8.8.8', port: 53, type: 'udp' },
timeout: 1000,
});

req.on('timeout', function () {
console.log('Timeout in making request');
...
```

#### <a name="apidoc.element.native-dns.client.Resolve"></a>[function <span class="apidocSignatureSpan">native-dns.client.</span>Resolve (opts, cb)](#apidoc.element.native-dns.client.Resolve)
- description and source-code
```javascript
function Resolve(opts, cb) {
  if (!(this instanceof Resolve)) return new Resolve(opts, cb);

  this.opts = util._extend({
    retryOnTruncate: true,
  }, opts);

  this._domain = opts.domain;
  this._rrtype = opts.rrtype;

  this._buildQuestion(this._domain);

  this._started = false;
  this._current_server = undefined;

  this._server_list = [];

  if (opts.remote) {
    this._server_list.push({
      address: opts.remote,
      port: 53,
      type: 'tcp',
    });
    this._server_list.push({
      address: opts.remote,
      port: 53,
      type: 'udp',
    });
  }

  this._request = undefined;
  this._type = 'getHostByName';
  this._cb = cb;

  if (!platform.ready) {
    _queue.push(this);
  } else {
    this.start();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.client.lookup"></a>[function <span class="apidocSignatureSpan">native-dns.client.</span>lookup (domain, family, callback)](#apidoc.element.native-dns.client.lookup)
- description and source-code
```javascript
lookup = function (domain, family, callback) {
  var rrtype, revip, res;

  if (!callback) {
    callback = family;
    family = undefined;
  }

  if (!family) {
    family = 4;
  }

  revip = net.isIP(domain);

  if (revip === 4 || revip === 6) {
    process.nextTick(function() {
      callback(null, domain, revip);
    });
    return {};
  }

  if (!domain) {
    process.nextTick(function() {
      callback(null, null, family);
    });
    return {};
  }

  rrtype = consts.FAMILY_TO_QTYPE[family];

  var opts = {
    domain: domain,
    rrtype: rrtype
  };

  res = new Lookup(opts);

  res._cb = function(err, response) {
    var i, afamily, address, a, all;

    if (err) {
      callback(err, undefined, undefined);
      return;
    }

    all = response.answer.concat(response.additional);

    for (i = 0; i < all.length; i++) {
      a = all[i];

      if (a.type === A || a.type === AAAA) {
        afamily = consts.QTYPE_TO_FAMILY[a.type];
        address = a.address;
        break;
      }
    }

    callback(err, address, afamily);
  };

  return res;
}
```
- example usage
```shell
...
};

Request.prototype.send = function() {
  debug('request starting', this.question);
  var self = this;

  if (this.cache && this.cache.lookup) {
    this.cache.lookup(this.question, function(results) {
var packet;

if (!results) {
  self._send();
} else {
  packet = new Packet();
  packet.answer = results.slice();
...
```

#### <a name="apidoc.element.native-dns.client.resolve"></a>[function <span class="apidocSignatureSpan">native-dns.client.</span>resolve (domain, rrtype, ip, callback)](#apidoc.element.native-dns.client.resolve)
- description and source-code
```javascript
resolve = function (domain, rrtype, ip, callback) {
  var res;

  if (!callback) {
    callback = ip;
    ip = undefined;
  }

  if (!callback) {
    callback = rrtype;
    rrtype = undefined;
  }

  rrtype = consts.NAME_TO_QTYPE[rrtype || 'A'];

  if (rrtype === PTR) {
    return reverse(domain, callback);
  }

  var opts = {
    domain: domain,
    rrtype: rrtype,
    remote: ip,
  };

  res = new Resolve(opts);

  res._cb = function(err, response) {
    var ret = [], i, a;

    if (err) {
      callback(err, response);
      return;
    }

    for (i = 0; i < response.answer.length; i++) {
      a = response.answer[i];
      if (a.type === rrtype) {
        switch (rrtype) {
          case A:
          case AAAA:
            ret.push(a.address);
            break;
          case consts.NAME_TO_QTYPE.MX:
            ret.push({
              priority: a.priority,
              exchange: a.exchange
            });
            break;
          case TXT:
          case NS:
          case CNAME:
          case PTR:
            ret.push(a.data);
            break;
          case SRV:
            ret.push({
              priority: a.priority,
              weight: a.weight,
              port: a.port,
              name: a.target
            });
            break;
          default:
            ret.push(a);
            break;
        }
      }
    }

    if (ret.length === 0) {
      ret = undefined;
    }

    callback(err, ret);
  };

  return res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.client.resolve4"></a>[function <span class="apidocSignatureSpan">native-dns.client.</span>resolve4 (domain, callback)](#apidoc.element.native-dns.client.resolve4)
- description and source-code
```javascript
resolve4 = function (domain, callback) {
  return resolve(domain, 'A', function(err, results) {
    callback(err, results);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.client.resolve6"></a>[function <span class="apidocSignatureSpan">native-dns.client.</span>resolve6 (domain, callback)](#apidoc.element.native-dns.client.resolve6)
- description and source-code
```javascript
resolve6 = function (domain, callback) {
  return resolve(domain, 'AAAA', function(err, results) {
    callback(err, results);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.client.resolveCname"></a>[function <span class="apidocSignatureSpan">native-dns.client.</span>resolveCname (domain, callback)](#apidoc.element.native-dns.client.resolveCname)
- description and source-code
```javascript
resolveCname = function (domain, callback) {
  return resolve(domain, 'CNAME', function(err, results) {
    callback(err, results);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.client.resolveMx"></a>[function <span class="apidocSignatureSpan">native-dns.client.</span>resolveMx (domain, callback)](#apidoc.element.native-dns.client.resolveMx)
- description and source-code
```javascript
resolveMx = function (domain, callback) {
  return resolve(domain, 'MX', function(err, results) {
    callback(err, results);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.client.resolveNs"></a>[function <span class="apidocSignatureSpan">native-dns.client.</span>resolveNs (domain, callback)](#apidoc.element.native-dns.client.resolveNs)
- description and source-code
```javascript
resolveNs = function (domain, callback) {
  return resolve(domain, 'NS', function(err, results) {
    callback(err, results);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.client.resolveSrv"></a>[function <span class="apidocSignatureSpan">native-dns.client.</span>resolveSrv (domain, callback)](#apidoc.element.native-dns.client.resolveSrv)
- description and source-code
```javascript
resolveSrv = function (domain, callback) {
  return resolve(domain, 'SRV', function(err, results) {
    callback(err, results);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.client.resolveTlsa"></a>[function <span class="apidocSignatureSpan">native-dns.client.</span>resolveTlsa (domain, callback)](#apidoc.element.native-dns.client.resolveTlsa)
- description and source-code
```javascript
resolveTlsa = function (domain, callback) {
  return resolve(domain, 'TLSA', function(err, results) {
    callback(err, results);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.client.resolveTxt"></a>[function <span class="apidocSignatureSpan">native-dns.client.</span>resolveTxt (domain, callback)](#apidoc.element.native-dns.client.resolveTxt)
- description and source-code
```javascript
resolveTxt = function (domain, callback) {
  return resolve(domain, 'TXT', function(err, results) {
    callback(err, results);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.client.reverse"></a>[function <span class="apidocSignatureSpan">native-dns.client.</span>reverse (ip, callback)](#apidoc.element.native-dns.client.reverse)
- description and source-code
```javascript
reverse = function (ip, callback) {
  var error, opts, res;

  if (!net.isIP(ip)) {
    error = new Error('getHostByAddr ENOTIMP');
    error.errno = error.code = 'ENOTIMP';
    throw error;
  }

  opts = {
    domain: utils.reverseIP(ip),
    rrtype: PTR
  };

  res = new Lookup(opts);

  res._cb = function(err, response) {
    var results = [];

    if (response) {
      response.answer.forEach(function(a) {
        if (a.type === PTR) {
          results.push(a.data);
        }
      });
    }

    if (results.length === 0) {
      results = undefined;
    }

    callback(err, results);
  };

  return res;
}
```
- example usage
```shell
...

    this._server_list.push(u);
    this._server_list.push(t);

    tries += 1;
  }

  this._server_list.reverse();
};

Resolve.prototype._popServer = function() {
  debug('resolve pop server', this._current_server, this._domain);
  this._server_list.splice(0, 1, this._current_server);
};
...
```



# <a name="apidoc.module.native-dns.consts"></a>[module native-dns.consts](#apidoc.module.native-dns.consts)

#### <a name="apidoc.element.native-dns.consts.nameToQtype"></a>[function <span class="apidocSignatureSpan">native-dns.consts.</span>nameToQtype (n)](#apidoc.element.native-dns.consts.nameToQtype)
- description and source-code
```javascript
nameToQtype = function (n) {
  return NAME_TO_QTYPE[n.toUpperCase()];
}
```
- example usage
```shell
...
'SRV',
'SOA',
'TLSA',
].forEach(function (type) {
exports[type] = function (opts) {
  var obj = {};
  opts = opts || {};
  obj.type = consts.nameToQtype(type);
  obj.class = consts.NAME_TO_QCLASS.IN;
  Object.keys(opts).forEach(function (k) {
    if (opts.hasOwnProperty(k) && ['type', 'class'].indexOf(k) == -1) {
      obj[k] = opts[k];
    }
  });
  return obj;
...
```

#### <a name="apidoc.element.native-dns.consts.qtypeToName"></a>[function <span class="apidocSignatureSpan">native-dns.consts.</span>qtypeToName (t)](#apidoc.element.native-dns.consts.qtypeToName)
- description and source-code
```javascript
qtypeToName = function (t) {
  return exports.QTYPE_TO_NAME[t];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.native-dns.packet"></a>[module native-dns.packet](#apidoc.module.native-dns.packet)

#### <a name="apidoc.element.native-dns.packet.packet"></a>[function <span class="apidocSignatureSpan">native-dns.</span>packet (socket)](#apidoc.element.native-dns.packet.packet)
- description and source-code
```javascript
packet = function (socket) {
  NDP.call(this);
  this.address = undefined;
  this._socket = socket;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.packet.parse"></a>[function <span class="apidocSignatureSpan">native-dns.packet.</span>parse (msg, socket)](#apidoc.element.native-dns.packet.parse)
- description and source-code
```javascript
parse = function (msg, socket) {
  var p = NDP.parse(msg);
  p._socket = socket;
  return p;
}
```
- example usage
```shell
...

  buff = this._socket.buffer(size);
  len = Packet.write(buff, this);
  this._socket.send(len);
};

Packet.parse = function (msg, socket) {
  var p = NDP.parse(msg);
  p._socket = socket;
  return p;
};

Packet.write = NDP.write;
...
```

#### <a name="apidoc.element.native-dns.packet.super_"></a>[function <span class="apidocSignatureSpan">native-dns.packet.</span>super_ ()](#apidoc.element.native-dns.packet.super_)
- description and source-code
```javascript
super_ = function () {
  this.header = {
    id: 0,
    qr: 0,
    opcode: 0,
    aa: 0,
    tc: 0,
    rd: 1,
    ra: 0,
    res1: 0,
    res2: 0,
    res3: 0,
    rcode: 0
  };
  this.question = [];
  this.answer = [];
  this.authority = [];
  this.additional = [];
  this.edns_options = [];   // TODO: DEPRECATED! Use '.edns.options' instead!
  this.payload = undefined; // TODO: DEPRECATED! Use '.edns.payload' instead!
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.packet.write"></a>[function <span class="apidocSignatureSpan">native-dns.packet.</span>write (buff, packet)](#apidoc.element.native-dns.packet.write)
- description and source-code
```javascript
write = function (buff, packet) {
  var state = WRITE_HEADER,
      val,
      section,
      count,
      rdata,
      last_resource,
      label_index = {};

  buff = new BufferCursor(buff);

  // the existence of 'edns' in a packet indicates that a proper OPT record exists
  // in 'additional' and that all of the other fields in packet (that are parsed by
  // 'parseOpt') are properly set. If it does not exist, we assume that the user
  // is requesting that we create one for them.
  if (typeof packet.edns_version !== 'undefined' && typeof packet.edns === "undefined")
    state = makeEdns(packet);

  // TODO: this is unnecessarily inefficient. rewrite this using a
  //       function table instead. (same for Packet.parse too).
  while (true) {
    try {
      switch (state) {
        case WRITE_HEADER:
          state = writeHeader(buff, packet);
          break;
        case WRITE_TRUNCATE:
          state = writeTruncate(buff, packet, section, last_resource);
          break;
        case WRITE_QUESTION:
          state = writeQuestion(buff, packet.question[0], label_index);
          section = 'answer';
          count = 0;
          break;
        case WRITE_RESOURCE_RECORD:
          last_resource = buff.tell();
          if (packet[section].length == count) {
            switch (section) {
              case 'answer':
                section = 'authority';
                state = WRITE_RESOURCE_RECORD;
                break;
              case 'authority':
                section = 'additional';
                state = WRITE_RESOURCE_RECORD;
                break;
              case 'additional':
                state = WRITE_END;
                break;
            }
            count = 0;
          } else {
            state = WRITE_RESOURCE_WRITE;
          }
          break;
        case WRITE_RESOURCE_WRITE:
          rdata = {};
          val = packet[section][count];
          state = writeResource(buff, val, label_index, rdata);
          break;
        case WRITE_RESOURCE_DONE:
          count += 1;
          state = writeResourceDone(buff, rdata);
          break;
        case WRITE_A:
        case WRITE_AAAA:
          state = writeIp(buff, val);
          break;
        case WRITE_NS:
        case WRITE_CNAME:
        case WRITE_PTR:
          state = writeCname(buff, val, label_index);
          break;
        case WRITE_SPF:
        case WRITE_TXT:
          state = writeTxt(buff, val);
          break;
        case WRITE_MX:
          state = writeMx(buff, val, label_index);
          break;
        case WRITE_SRV:
          state = writeSrv(buff, val, label_index);
          break;
        case WRITE_SOA:
          state = writeSoa(buff, val, label_index);
          break;
        case WRITE_OPT:
          state = writeOpt(buff, val);
          break;
        case WRITE_NAPTR:
          state = writeNaptr(buff, val, label_index);
          break;
        case WRITE_TLSA:
          state = writeTlsa(buff, val);
          break;
        case WRITE_END:
          return buff.tell();
        default:
          if (typeof val.data !== 'object')
            throw new Error('Packet.write Unknown State: ' + state);
          // write unhandled RR type
          buff.copy(val.data);
          state = WRITE_RESOURCE_DONE;
      }
    } catch (e) {
      if (e instanceof BufferCursorOverflow) {
        state = WRITE_TRUNCATE;
      } else {
        throw e;
      }
    }
  }
}
```
- example usage
```shell
...
if (typeof(this.edns_version) !== 'undefined') {
  size = 4096;
}

this.payload = size = size || this._socket.base_size;

buff = this._socket.buffer(size);
len = Packet.write(buff, this);
this._socket.send(len);
};

Packet.parse = function (msg, socket) {
var p = NDP.parse(msg);
p._socket = socket;
return p;
...
```



# <a name="apidoc.module.native-dns.packet.prototype"></a>[module native-dns.packet.prototype](#apidoc.module.native-dns.packet.prototype)

#### <a name="apidoc.element.native-dns.packet.prototype.send"></a>[function <span class="apidocSignatureSpan">native-dns.packet.prototype.</span>send ()](#apidoc.element.native-dns.packet.prototype.send)
- description and source-code
```javascript
send = function () {
  var buff, len, size;

  if (typeof(this.edns_version) !== 'undefined') {
    size = 4096;
  }

  this.payload = size = size || this._socket.base_size;

  buff = this._socket.buffer(size);
  len = Packet.write(buff, this);
  this._socket.send(len);
}
```
- example usage
```shell
...
});

req.on('end', function () {
 var delta = (Date.now()) - start;
 console.log('Finished processing request: ' + delta.toString() + 'ms');
});

req.send();
'''

Request creation takes an object with the following fields

* 'question' -- an instance of Question (required)
* 'server' -- defines the remote end point (required)
 - as an object it should be
...
```



# <a name="apidoc.module.native-dns.pending"></a>[module native-dns.pending](#apidoc.module.native-dns.pending)

#### <a name="apidoc.element.native-dns.pending.remove"></a>[function <span class="apidocSignatureSpan">native-dns.pending.</span>remove (request)](#apidoc.element.native-dns.pending.remove)
- description and source-code
```javascript
remove = function (request) {
  var hash = serverHash(request.server);
  var socket = _sockets[hash];
  if (socket) {
    socket.remove(request);
  }
}
```
- example usage
```shell
...
}
};

Request.prototype.done = function() {
debug('request finished', this.id, this.question);
this.fired = true;
clearTimeout(this.timer_);
PendingRequests.remove(this);
this.emit('end');
this.id = undefined;
};

Request.prototype.handleTimeout = function() {
if (!this.fired) {
  debug('request timedout', this.id, this.question);
...
```

#### <a name="apidoc.element.native-dns.pending.send"></a>[function <span class="apidocSignatureSpan">native-dns.pending.</span>send (request)](#apidoc.element.native-dns.pending.send)
- description and source-code
```javascript
send = function (request) {
  var hash = serverHash(request.server);
  var socket = _sockets[hash];

  if (!socket) {
    switch (hash) {
      case 'udp4':
      case 'udp6':
        socket = new SocketQueue(new UDPSocket(), hash);
        break;
      default:
        socket = new SocketQueue(new TCPSocket(), request.server);
        break;
    }

    socket.on('close', function() {
      delete _sockets[hash];
    });

    _sockets[hash] = socket;
  }

  socket.send(request);
}
```
- example usage
```shell
...
});

req.on('end', function () {
 var delta = (Date.now()) - start;
 console.log('Finished processing request: ' + delta.toString() + 'ms');
});

req.send();
'''

Request creation takes an object with the following fields

* 'question' -- an instance of Question (required)
* 'server' -- defines the remote end point (required)
 - as an object it should be
...
```



# <a name="apidoc.module.native-dns.server"></a>[module native-dns.server](#apidoc.module.native-dns.server)

#### <a name="apidoc.element.native-dns.server.createServer"></a>[function <span class="apidocSignatureSpan">native-dns.server.</span>createServer (opts)](#apidoc.element.native-dns.server.createServer)
- description and source-code
```javascript
createServer = function (opts) {
  return new UDPServer(opts || {});
}
```
- example usage
```shell
...
Server
------

There is also a rudimentary server implementation

'''javascript
var dns = require('../dns'),
server = dns.createServer();

server.on('request', function (request, response) {
//console.log(request)
response.answer.push(dns.A({
  name: request.question[0].name,
  address: '127.0.0.1',
  ttl: 600,
...
```

#### <a name="apidoc.element.native-dns.server.createTCPServer"></a>[function <span class="apidocSignatureSpan">native-dns.server.</span>createTCPServer (opts)](#apidoc.element.native-dns.server.createTCPServer)
- description and source-code
```javascript
createTCPServer = function (opts) {
  return new TCPServer(opts || {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.server.createUDPServer"></a>[function <span class="apidocSignatureSpan">native-dns.server.</span>createUDPServer (opts)](#apidoc.element.native-dns.server.createUDPServer)
- description and source-code
```javascript
createUDPServer = function (opts) {
  return exports.createServer(opts);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.native-dns.utils"></a>[module native-dns.utils](#apidoc.module.native-dns.utils)

#### <a name="apidoc.element.native-dns.utils.TCPSocket"></a>[function <span class="apidocSignatureSpan">native-dns.utils.</span>TCPSocket (socket)](#apidoc.element.native-dns.utils.TCPSocket)
- description and source-code
```javascript
TCPSocket = function (socket) {
  UDPSocket.call(this, socket);
  this.base_size = 4096;
  this._rest = undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.utils.UDPSocket"></a>[function <span class="apidocSignatureSpan">native-dns.utils.</span>UDPSocket (socket, remote)](#apidoc.element.native-dns.utils.UDPSocket)
- description and source-code
```javascript
UDPSocket = function (socket, remote) {
  this._socket = socket;
  this._remote = remote;
  this._buff = undefined;
  this.base_size = 512;
  this.bound = false;
  this.unref = undefined;
  this.ref = undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.native-dns.utils.reverseIP"></a>[function <span class="apidocSignatureSpan">native-dns.utils.</span>reverseIP (ip)](#apidoc.element.native-dns.utils.reverseIP)
- description and source-code
```javascript
reverseIP = function (ip) {
  var address, kind, reverseip, parts;
  address = ipaddr.parse(ip.split(/%/)[0]);
  kind = address.kind();

  switch (kind) {
    case 'ipv4':
      address = address.toByteArray();
      address.reverse();
      reverseip = address.join('.') + '.IN-ADDR.ARPA';
      break;
    case 'ipv6':
      parts = [];
      address.toNormalizedString().split(':').forEach(function(part) {
        var i, pad = 4 - part.length;
        for (i = 0; i < pad; i++) {
          part = '0' + part;
        }
        part.split('').forEach(function(p) {
          parts.push(p);
        });
      });
      parts.reverse();
      reverseip = parts.join('.') + '.IP6.ARPA';
      break;
  }

  return reverseip;
}
```
- example usage
```shell
...
if (!net.isIP(ip)) {
  error = new Error('getHostByAddr ENOTIMP');
  error.errno = error.code = 'ENOTIMP';
  throw error;
}

opts = {
  domain: utils.reverseIP(ip),
  rrtype: PTR
};

res = new Lookup(opts);

res._cb = function(err, response) {
  var results = [];
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
