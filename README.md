# ipecho [![Codecov](https://img.shields.io/codecov/c/github/Eun/coredns-ipecho.svg)]() [![Travis](https://img.shields.io/travis/Eun/coredns-ipecho.svg)]()
*ipecho* is an [coredns](https://github.com/coredns/coredns/) plugin, it answers ip subdomain queries with the ip itself.

## Example
```
A IN 127.0.0.1.example.com. -> A: 127.0.0.1
AAAA IN ::1.example.com. -> AAAA: ::1
```

## Syntax
```
ipecho {
    domain example1.com
    domain example2.com
    ttl 2629800
}
```

* **domain** adds the domain that should be handled
* **ttl** defines the ttl that should be used in the response
* **debug** enables debug logging