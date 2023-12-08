Identities are given as a URL.

* trustsocially.org
* trustsocially.org/p/philipcristiano

A "root" path of a domain or a domain with path `/`

Optionally a path component of more than `/` can be used for multiple identities at the same domain

## Requirements

Requests MUST be over HTTPS.

## Order to check for trust.txt

### When given a root path identity

A root path identity should check for

1) `/.well-known/trust.txt`
2) `/trust.txt`
3) `link` element in the identity resource HTML with `rel=trust`.

### When given a non-root path identity

1) `link` element in the identity resource HTML with `rel=trust`.
