# Chapter 3 — Advanced Libraries

## Exec — Run Commands

```cajyu
import exec from CajyuLibs.exec;

var files = exec.exec("ls");
print(files);
```

## HTTP — Servers

```cajyu
import Server from CajyuLibs.http;

var server = new Server(3000);
server.file("/", "<h1>Hello from Cajyu</h1>");
```

## HTTP Part 2 — POST, GET and Sleep

```cajyu
server.post(fn body {
  return { code: 200, result: body.a + body.b };
});

server.sleep();
server.wake();
```

## WebSockets — How and Why

WebSockets let you send and receive messages in real time.

```cajyu
import WS from CajyuLibs.websocket;

var wss = new WS.Server(8080);

wss.on("connection", fn client {
  print("Client connected");
});

wss.on("message", fn msg {
  wss.broadcast(msg);
});
```

Next: [Chapter 4 — Bigger Projects](../Chapter-4/)
