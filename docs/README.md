# cosmoterm

Terminal messenger using p2p technologies
(project is currently *in development*)

![logo](https://github.com/IvanIsak2000/cosmoterm/assets/79650307/44c94073-9c72-4edc-93a1-9e6308b72da0)





## Usage HOWTO

### Read messages

1. Enable it yourself

```bash
python3 server.py
```
OR

2. Install `server.py ` in startup

```bash
python3 main.py --set
```

### Send messages
```bash
python3 main.py --send <host> <port> <password>
```

<hr>

## Example

### 1. Await
To receive a message, you need to enable the server part of the program:

![server main ](https://github.com/IvanIsak2000/cosmoterm/assets/79650307/03c5d54d-1097-4362-b56f-8de109120109)

![qr](https://github.com/IvanIsak2000/cosmoterm/assets/79650307/97a3a61c-0e94-49c5-ab60-47da06174c40)



>The QR code is created from your "host", "port" and the "password" automatically created for the current session, and then all this is recorded in the QR code



### 2. Send

Let's say we want to send a message to a friend, for this open the terminal and write:
```bash 

python3 main.py --send <host> <port> <password>

```

### 3. Connection

The server is waiting for the connection

>`server.py`
>
>![wait](https://github.com/IvanIsak2000/cosmoterm/assets/79650307/effd7a5d-1411-464b-a055-b732226c2a5d)

>`main.py` 
>
>![image](https://github.com/IvanIsak2000/cosmoterm/assets/79650307/aed473c8-d8bd-431b-b634-0c7ea8a582fa)



### 4. Check token and get messege

>`server.py`
>
>![server](https://github.com/IvanIsak2000/cosmoterm/assets/79650307/ca459917-67c2-448f-8d9c-e8bf0bc35290)


>`main.py`
>
>![main](https://github.com/IvanIsak2000/cosmoterm/assets/79650307/5b03a0ed-2803-4316-9754-157c20efca86)


### 5. Add in `history.toml`,`client.log` and `server.log`(automatically)
       
```
#history.toml
[friend host]
"2023-05-23 09:15:58" = "Hi!"     
 ```
 
 ```
 #server.log
 023-05-23 09:21:53,459 INFO __main__ ('192.168.0.139', 24043): Hi! True
 
 ```
 
 ```
 #client.log
 2023-05-23 09:31:39,234 INFO __main__ 192.168.0.139: Hi
 
 ```
 
       


## Found a bug?

It's possible to submit a bug report or a feature request via GitHub [issues](https://github.com/IvanIsak2000/cosmoterm/issues/new)

## Contribution

Checkout [contributing guidelines](docs/CONTRIBUTING.md)





