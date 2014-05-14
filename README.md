nginxibition
============

Nginx can do a lot of neat things, most of which I had *no idea* about until recently. It is time to uncover some **nginxcellence**.

# Nginx Tomfoolery as a Service

This is a collection of nginx silliness. If you have something wacky that needs to end up as part of an nginx configuration, please add it here.

## Where am I :white_check_mark:

Returns GeoJSON with lon/lat using the client's IP with the geoip module. 

```bash
curl http://23.253.232.101/whereami
{ "type": "Feature", "geometry": { "type": "Point", "coordinates": [-98.3987, 29.4889] }, "properties": { "ip": "23.253.232.101" } }
```

GeoIPs are almost always off, but hey this is just for fun. The IP below is actually around Dallas, TX but the coordinates given are for San Antonio, TX (home base of Rackspace, who owns the IP address).

## [Hyper Text Coffee Pot Control Protocol](http://en.wikipedia.org/wiki/Hyper_Text_Coffee_Pot_Control_Protocol) :white_check_mark:

HTTP proxy for coffeepots, in nginx configuration.

Getting coffee is easy:

```bash
$ curl -X BREW http://23.253.232.101/coffee
Brewing coffee.
$ curl http://23.253.232.101/coffee
Your coffee is served.
```

There are more commands you can send the coffeepot. Try for yourself, add more in a PR.

# Must play with later

* [Postgres for nginx](https://github.com/FRiCKLE/ngx_postgres/)
 * Use it to create a [simple API to a database](http://rny.io/nginx/postgresql/2013/07/26/simple-api-with-nginx-and-postgresql.html). What could possibly go wrong?
* Redis for nginx
* Memcached for nginx

Why do these things exist? Who knows, who cares? Now I can connect nginx to my database.
Forget applications, my nginx configuration *is* my app.


