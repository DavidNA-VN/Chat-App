# Chat-App

Desktop chat application with an Electron and TypeScript client and a C server.
The client connects directly over TCP using Node.js `node:net`. The server uses
non-blocking POSIX sockets and `poll()` to handle multiple connections and SQLite3
for persistence. A custom application protocol defines message framing over TCP.

## Repository layout

| Path | Purpose |
| --- | --- |
| `server/src/` | C server implementation |
| `server/include/` | Server headers |
| `server/tests/` | Server tests |
| `client/src/` | Electron and TypeScript client source |
| `protocol/` | Application protocol and framing specification |
| `database/` | SQLite schema and migrations |
| `docs/` | Project documentation |
| `tests/` | Cross-component integration tests |
