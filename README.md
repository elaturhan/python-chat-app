# Python Chat Application

A terminal-based TCP chat learning project by Ela Turhan, using Python's built-in `socket` and `threading` modules.

## Features

- A server accepts multiple clients and broadcasts messages.
- Clients choose nicknames and send and receive messages using separate threads.
- Join notifications are broadcast to connected clients.

## Run locally

Python 3 is required. No third-party packages are needed.

Start the server in a terminal:

```sh
python server.py
```

In two or more additional terminals, start a client:

```sh
python client.py
```

Choose a nickname in each client, then type a message and press Enter. The default address is `127.0.0.1:55555`, so run all processes on the same computer. Stop them with Ctrl+C.

## Files

- `server.py`: connection handling and message broadcasting.
- `client.py`: nickname entry, message sending and receiving.

## Scope

The original source files are preserved. This is a local networking exercise; robust disconnect handling, TCP message framing and synchronization of shared client lists remain areas for improvement. Authentication and encryption are not implemented.
