# Solana - Create Your Own Crypto


```
$ solana-keygen new
$ solana-keygen new --force
$ solana balance --url devnet
$ solana airdrop 2 [ADDRESS] --url devnet

$ solana config get
$ solana config set --url [https://api.devnet.solana.com or devnet]
```

## Need Spl-token-cli library
Require the library for creating and minting tokens.

```
$ spl-token create-token --url devnet
$ spl-token create-account [TOKEN_ADD] --url devnet

$ spl-token mint [TOKEN_ADD] --url devnet
$ spl-token supply [TOKEN_ADD] --url devnet

$ spl-token authorize [TOKEN_ADD] mint --disable --url devnet

$ spl-token burn [TOKEN_ACCOUNT_ADD] 1000 --url devnet
$ spl-token balance [TOKEN_ADD] --url devnet
```
## Are you having error? libssl-dev 
Error: spl-token: error while loading shared libraries: libssl.so.1.1: cannot open shared object file: No such file or directory

```
$ wget http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/libssl1.1_1.1.1-1ubuntu2.1~18.04.20_amd64.deb 


$ sudo dpkg -i libssl1.1_1.1.1-1ubuntu2.1~18.04.20_amd64.deb
```

-> [Solution Reference](https://github.com/dotnet/sdk/issues/24759)

