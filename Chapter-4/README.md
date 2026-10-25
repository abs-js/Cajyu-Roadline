# Chapter 4 — Bigger Projects

## Starting a Bigger Server

Combine HTTP routes, static files and logic.

## World Click Counter

A button that counts clicks from anyone who visits.

## Live Chat

Chat using WebSocket + ReadLine for the server side.

## Digital Menu

A simple restaurant menu served with Cajyu.

### Example: Simple Menu Server

```cajyu
import Server from CajyuLibs.http;

var server = new Server(3000);

var menu = "<h1>Menu</h1><ul><li>Pizza</li><li>Salad</li></ul>";
server.file("/", menu);
```

Congratulations! You finished the Cajyu Roadline.
