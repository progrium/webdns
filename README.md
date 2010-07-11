# WebDNS

A protocol and implementation for doing DNS over HTTP. It's a work in progress. 

## WebDNS Gateway

This gateway is a DNS server and WebDNS client. It allows you to serve DNS queries via HTTP to DNS via this gateway.

Run on port 1053 with:

`PORT=1053 python ./gateway`

By default this points to the Domdori WebDNS server, which is a non-recursive, authoritative DNS host for Domdori user. You can point to another WebDNS server with:

`PORT=1053 BASE_URL=http://yourdomain.com/dns python ./gateway`

## WebDNS Server

As you might expect, a WebDNS server is just a web server/application. For a reference implementation see this [App Engine module for Domdori](http://github.com/progrium/domdori/blob/master/dns.py). 

## More

This work is a collaboration of Joel Franusic and Jeff Lindsay for the [Domdori](http://github.com/progrium/domdori) project. Joel's work on this project is [here](http://github.com/jpf/jsondns)