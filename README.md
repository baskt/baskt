# Baskt

Baskt is a president cloud-based key/value storage solution perfect for fast
development, prototyping and testing of web and mobile applications.

### Create a new baskt
```bash
> curl -X POST https://baskt.xyz
```

#### Response
{
    "baskt": "d5192d9db7a64fd98681df3cdaad10cf"
}

### To load all key/value pairs from baskt
```bash
> curl https://baskt.xyz/<baskt_key>
```

#### Response
{
    "baskt": "d5192d9db7a64fd98681df3cdaad10cf",
    "data": {
        "key": "value"
    }
}

### Save key/value pair
```bash
> curl -X PUT -d 'data' https://baskt.xyz/<baskt_key>/<key>
```

#### Response
{
    "baskt": "d5192d9db7a64fd98681df3cdaad10cf"
    "saved": "key"
}

### To retrieve a value for a given key, create a 'get' request.
```bash
> curl https://baskt.xyz/<baskt_key>/<key>
```

#### Response
{
    "baskt": "d5192d9db7a64fd98681df3cdaad10cf",
    "key": "value"
}

### To delete a key, create a 'delete' request.
```bash
> curl -X DELETE https://baskt.xyz/<baskt_key>/<key>
```

#### Response
{
    "baskt": "d5192d9db7a64fd98681df3cdaad10cf",
    "deleted": "key"
}

## Notice

All baskts which are not accessed for more than 30 days will be removed.

## Libraries

- Python - https://github.com/baskt/baskt-python

##  How to Contribute

We encourage contribution to our libraries. Please submit your ideas and requests
to us via hello@baskt.xyz or by creating a new issue in the issue tracker (preferred).
- Please search for existing issues in order to ensure we don't have any duplicates.
- Respect and be considerate of others when commenting.
