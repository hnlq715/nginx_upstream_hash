NOTE: This module is obsolete as of Nginx 1.7.2, which includes the [hash](http://nginx.org/r/hash) directive. This repository remains for historical interest only.
==

ngx_http_upstream_hash_module
--

Installation:

    cd nginx-0.7.62 # or whatever
    ./configure --add-module=/path/to/this/directory
    make
    make install

Usage:

    upstream backend {
        ...
        hash        $request_uri;
        hash_again  10;          # default 0
    }

Works the same on 32-bit and 64-bit systems.

See http://wiki.nginx.org/NginxHttpUpstreamRequestHashModule for more details.

Questions/patches to Evan Miller, emmiller@gmail.com.
