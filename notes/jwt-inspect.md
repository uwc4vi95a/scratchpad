# JWT Inspection

Quick way to decode a JWT payload from the command line:

```sh
echo "$JWT" | cut -d. -f2 | base64 -d 2>/dev/null
```

For HMAC-signed tokens, verify with `jq` and `openssl`.

Remember: never log tokens in production.
