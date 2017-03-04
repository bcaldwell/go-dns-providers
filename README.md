# go-dns-providers

go-dns-providers is a fork of [xenolf/lego/providers/dns](https://github.com/xenolf/lego). The goal of this project is to decouple the dns providers from the rest of the lego project. In addition the following functions will be exposed:
  - `CreateDnsEntry` to create a new dns entry
  - `DeleteDnsEntry` to delete an extisting dns entry

For use with [crypto/acme](https://godoc.org/golang.org/x/crypto/acme) the following function will be exposed:
  - `challengeSetup` to create dns entry to pass challenge
  - `challengeCleanup` to remove dns challenge entry
  
