cert
====


## Overview
cert is command line utility to generate a self-signed X.509 certificate
for a TLS server. Outputs to `cert.pem` and `key.pem` and will overwrite
existing files. It is based on the [generate-cert](http://golang.org/src/pkg/crypto/tls/generate_cert.go)
tool included with the go source -- only slightly modified to take more arguments.

## Prerequisites
None, binaries are statically linked.
If you want to compile from source you need the [go toolchain](http://golang.org/doc/install).

## Installation
- Save binary to a location in your PATH (i.e. `/usr/local/bin/`)

### Downloads
- [cert-darwin-386.tar.gz](https://drive.google.com/uc?id=0B3X9GlR6EmbnamJlTThOR1pTbEk)
- [cert-darwin-amd64.tar.gz](https://drive.google.com/uc?id=0B3X9GlR6EmbnT0VyLTlwUnVlQWc)
- [cert-freebsd-386.tar.gz](https://drive.google.com/uc?id=0B3X9GlR6EmbneTZFUWJuUV9pSWs)
- [cert-freebsd-amd64.tar.gz](https://drive.google.com/uc?id=0B3X9GlR6EmbnTGFnNWlNeHZROW8)
- [cert-linux-386.tar.gz](https://drive.google.com/uc?id=0B3X9GlR6EmbnR0g0MV9hbl9tVDg)
- [cert-linux-amd64.tar.gz](https://drive.google.com/uc?id=0B3X9GlR6EmbnR1gzSGZrMHpqdXc)
- [cert-linux-arm.tar.gz](https://drive.google.com/uc?id=0B3X9GlR6EmbnOVJldWtfcUl1QTg)
- [cert-linux-arm5.tar.gz](https://drive.google.com/uc?id=0B3X9GlR6EmbnUWlyRjIyLTRWV2s)
- [cert-windows-386.tar.gz](https://drive.google.com/uc?id=0B3X9GlR6Embnd1hiemRoQ0djT2c)
- [cert-windows-amd64.tar.gz](https://drive.google.com/uc?id=0B3X9GlR6EmbnTE1hNzRMNEc4UW8)

## Example

###### Generate a self-signed certificate valid for 1 year
    $ cert -host example.com -org "Acme Co" -years 1
    2013/02/02 16:45:56 written cert.pem
    2013/02/02 16:45:56 written key.pem
