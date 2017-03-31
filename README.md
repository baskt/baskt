# Baskt

Baskt is a president cloud-based key/value storage solution perfect for fast
development, prototyping and testing of web and mobile applications.

```bash
# Create a new baskt
> curl -X POST https://baskt.xyz
d5192d9db7a64fd98681df3cdaad10cf

# To load all key/value pairs from baskt
> curl https://baskt.xyz/baskt_key
{"key1": "value", "key2": "value2"}

# Save key/value pair
> curl -X PUT -d 'data' https://baskt.xyz/<baskt_key>/<key>

# To retrieve a value for a given key, create a 'get' request.
> curl https://baskt.xyz/<baskt_key>/<key>
value

# To delete a key, create a 'delete' request.
$ curl -X DELETE https://baskt.xyz/<baskt_key>/<key>
```

## Libraries

- Python - https://github.com/baskt/baskt-python
