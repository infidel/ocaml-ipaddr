# ocaml-ipaddr

A library for manipulation of IP (and MAC) address representations.

Features:

 * Depends only on sexplib (conditionalization under consideration)
 * oUnit-based tests
 * IPv4 and IPv6 support
 * IPv4 and IPv6 CIDR prefix support
 * IPv4 and IPv6 [CIDR-scoped address](http://tools.ietf.org/html/rfc4291#section-2.3) support
 * `Ipaddr.V4` and `Ipaddr.V4.Prefix` modules are `Map.OrderedType`
 * `Ipaddr.V6` and `Ipaddr.V6.Prefix` modules are `Map.OrderedType`
 * `Ipaddr` and `Ipaddr.Prefix` modules are `Map.OrderedType`
 * `Ipaddr_unix` in findlib subpackage `ipaddr.unix` provides compatibility with the standard library `Unix` module
 * `Ipaddr_top` in findlib subpackage `ipaddr.top` provides top-level pretty printers (requires compiler-libs default since OCaml 4.0)
 * IP address scope classification
 * IPv4-mapped addresses in IPv6 (::ffff:0:0/96) are an embedding of IPv4
 * MAC-48 (Ethernet) address support
 * `Macaddr` is a `Map.OrderedType`
 * All types have sexplib serializers/deserializers
