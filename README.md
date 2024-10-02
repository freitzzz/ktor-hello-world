# ktor-hello-world

Really simple counter built with ktor + moustache.

## Notes

- Used JDK: Amazon Corretto 22
- Used embedded server: Netty
- Avg startup memory usage: 100MB
- Avg memory usage with 100~400 RPS: 132MB
- Avg memory usage with 900~2000 RPS: 300MB
  - Traced memory usage with Visual VM, and it seems this happens because netty caches request headers.