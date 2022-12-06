install rustup

```sh
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

set flag for target native
```sh
RUSTFLAGS='-C target-cpu=native'
```