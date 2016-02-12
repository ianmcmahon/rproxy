# rproxy

## Rewriting reverse proxy library for Go

This is based on the code in the go standard library at net/http/httputil/reverseproxy.go

One addition was made, which is to provide a BodyRewriter hook to users to override the default body copy function with a Rewriter interface, allowing users to intercept the response and rewrite as necessary.
