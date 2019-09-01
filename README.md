# Sockets

Yet another simple socket client/server approach in python.

### Motivation

* Sockets provide a simple and supported form of IPC (Inter Proccess Comunication) for use throught all your computer
* Sockets can be implemented/used cross-languages or even cross-OS
* `Python` is one of the simple languages that can be used even for scripting

### Usage

You will need 2 windows (or tabs/panes) from terminal. Run the server first

```sh
$ python server.py
```

And then run the client

```sh
$ python client.py
```

On the client side you can send messages typing the terminal. If you want to see the server sending messages, you can enable with the flags:

```python
# client.py
RECV_DATA_FROM_SERVER = True

# server.py
SEND_DATA_TO_CLIENT = True
```

And the server will respond with `Server Ok!` message.


### FAQ

*Question: Is my server runnning?*

If you need to see if your server are actually running, try running

```sh
$ netstat -an | grep ${PORT}
```

The default port is `65432`, but you may have another port


* [Reference](https://realpython.com/python-sockets/)
