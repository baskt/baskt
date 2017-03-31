# Baskt

Baskt is a president cloud-based key/value storage solution perfect for fast
development, prototyping and testing of web and mobile applications.

### Create a new baskt
```bash
> curl -X POST https://baskt.xyz
```
d5192d9db7a64fd98681df3cdaad10cf

### To load all key/value pairs from baskt
```bash
> curl https://baskt.xyz/baskt_key
```
{"key1": "value", "key2": "value2"}

### Save key/value pair
```bash
> curl -X PUT -d 'data' https://baskt.xyz/<baskt_key>/<key>
```

### To retrieve a value for a given key, create a 'get' request.
```bash
> curl https://baskt.xyz/<baskt_key>/<key>
```
value

### To delete a key, create a 'delete' request.
```bash
$ curl -X DELETE https://baskt.xyz/<baskt_key>/<key>
```

## Libraries

- Python - https://github.com/baskt/baskt-python
