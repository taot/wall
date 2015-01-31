# Shadowsocks

## Basic Usage

This guide shows a very basic usage of shadowsock.

### Server Side

Unzip *shadowsocks-server-linux64-[version].gz*, and put the extracted binary to anywhere you like, and execute the following command:

```
./shadowsocks-server -d=true -p=23456 -k=password
```
where -p specifies the server port, -k specifies the password, both of which are required. And -d=true tells it to print out debug messages.

### Client Side

Unzip *shadowsocks-local-linux64-[version].gz*, and execute the following command:

```
./shadowsocks-local -k=qazwsx$#@! -l=23456 -p=23456 -s=54.191.101.209 -d=true
```

where -k specifies the password, -l specifies the local socks5 proxy port, -p specifies the server port, -s specifies server address.

