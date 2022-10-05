# socket_chat


Encrypted Chat (python) Curses for Terminal !!

---
>Easy to use 

>Inbuilt Encryption

>TCP socket

>Terminal UI

## installation
```
git clone https://github.com/security-softwares/socket_chat/

cd socket_chat

python3 chat_server -h

```

### For joining server 
- >python3 chat_client.py

 For public server use
Ngrok and local Host and local Port 
# **OR**

## Tor setup over chat traffic

>nano /etc/tor/torrc
- **remove "#" from these lines**
```

HiddenServiceDir /var/lib/tor/hidden_service/
HiddenServicePort 80 127.0.0.1:8080
                   ^             ^
                   |             |
                   |     set any port to listen 
                         
  Note:    these port should not be same 
```
- >sudo cat /var/lib/tor/hidden_service/hostname
- **copy host address**
- *after all configurations completed*

# **TO Run in Tor Network**

## Server Side Tor

- >torsocks python3 chat_server.py

host=localhost or (default)

port = 8080 ``` as set in the torrc ```


## Client side Tor

- >torsocks python3 chat_client.py

host= hostname (.onion address)

port = 80 ``` listning address of tor ```

