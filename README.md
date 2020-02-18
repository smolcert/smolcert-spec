# smolcert  [![CircleCI](https://circleci.com/gh/connctd/smolcert/tree/master.svg?style=svg)](https://circleci.com/gh/connctd/smolcert/tree/master) [![codecov](https://codecov.io/gh/connctd/smolcert/branch/master/graph/badge.svg)](https://codecov.io/gh/connctd/smolcert) [![GoDoc](https://godoc.org/github.com/connctd/smolcert?status.svg)](https://godoc.org/github.com/connctd/smolcert)

smolcert is an implementation of [CBOR](https://cbor.io) based certificates inspired by
[CBOR Profile of X.509 Certificates](https://tools.ietf.org/id/draft-raza-ace-cbor-certificates-00.html).

The goal is to have a more compact and easier to parse (especially on embedded systems) certificate format
than X.509. The certificate format is specified as [CDDL](https://tools.ietf.org/html/rfc8610) in the file
`spec.cddl`. Generated binary encoded certificates can be verified against this specification.

Currently exist implementations in [go](https://github.com/smolcert/smolcert-go) 
and [Rust](https://github.com/smolcert/smolcert-rust), where the go implementation is the more complete,
with support for easy certificate creation, signing and validation. The Rust implementation currently
only supports serialization and deserialization of certificates, signing and verification.

