# Baskt

Baskt is a president cloud-based key/value storage solution perfect for fast
development, prototyping and testing of web and mobile applications.

```bash
# Create a new baskt
$ curl -X POST https://baskt.xyz

# To load all key/value pairs from baskt
$ curl https://baskt.xyz/baskt_key

# Save key/value pair
# baskt_key: your baskt key
# key: property key
# value: value of key is sent as a --data parameter
$ curl -X PUT -d 'data' https://baskt.xyz/<baskt_key>/<key>

# To retrieve a value for a given key, create a 'get' request.
# baskt_key: your baskt key
# key: property key to retrieve
$ curl https://baskt.xyz/<baskt_key>/<key>

# To delete a key, create a 'delete' request.
# baskt_key: your baskt key
# key: property key to delete
$ curl -X DELETE https://baskt.xyz/<baskt_key>/<key>
```

## Libraries

- Python - https://github.com/baskt/baskt-python
