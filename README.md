nodejitsu-wss
=============

Quick example app to show how to deploy a websocket app using wss:// on
nodejitsu

Do it
-----
1. npm install
2. edit package.json:

```javascript
    "name": "<your app name>",
    "subdomain": "<your subdomain>",
    "version": "<your version>",
```
3. edit index.html:

```javascript
    io.connect('wss://<your subdomain>.nodejitsu.com');
```
4. jitsu deploy

Test it
-------

1. sudo node server.js
2. open http://localhost/
3. click "connect"

It should show the messages in the console log, which means it communicated to
your nodejitsu.com subdomain over wss://
