nginxibition
============

Nginx can do a lot of neat things.

While trying to fix an issue on some production servers, I noticed some nginx features I never touch but were just begging to be played with.

# Nginx Tomfoolery as a Service

## Where am I :white_check_mark:

Returns GeoJSON with lon/lat using the client's IP with the geoip module

## [Hyper Text Coffee Pot Control Protocol](http://en.wikipedia.org/wiki/Hyper_Text_Coffee_Pot_Control_Protocol) :white_check_mark:

HTTP proxy for coffeepots, in nginx configuration.

Getting coffee is easy:

```bash
$ curl -X BREW http://23.253.232.101/coffee
Brewing coffee.
$ curl http://23.253.232.101/coffee
Your coffee is served.
```

# Must play with later

* Postgres for nginx
* Redis for nginx
* Memcached for nginx

Why do these things exist? Who knows, who cares? Now I can connect nginx to my database.
Forget applications, my nginx configuration *is* my app.


