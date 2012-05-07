nodejitsu-wss
=============

Quick example app to show how to deploy a websocket app using wss:// on
nodejitsu

Do it
-----
1. npm install
2. edit package.json
    "name": "<your app name>",
    "subdomain": "<your subdomain>",
    "version": "<your version>",
3. edit index.html
    io.connect('wss://<your subdomain>.nodejitsu.com');
4. jitsu deploy
