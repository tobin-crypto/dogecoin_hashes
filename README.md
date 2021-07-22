# Dogecoin Hashes Library

This repository was forked from
[bitcoin_hashes](https://github.com/rust-bitcoin/bitcoin_hashes) in an effort
to work with Dogecoin in Rust.

The dogecoin patchset is extremely small, currently all we do is:

- Add this section to the README.
- Rename the package.
- Depend upon [rust-dogecoin](https://github.com/tobin-crypto/rust-dogecoin)
  (dogecoin fork of
  [rust-bitcoin](https://github.com/rust-bitcoin/rust-bitcoin)).

## ----- Original bitcoin_hashes README ------

[![Status](https://travis-ci.org/rust-bitcoin/bitcoin_hashes.png?branch=master)](https://travis-ci.org/rust-bitcoin/bitcoin_hashes)

# Bitcoin Hashes Library

This is a simple, no-dependency library which implements the hash functions
needed by Bitcoin. These are SHA1, SHA256, SHA256d, SHA512, and RIPEMD160. As an
ancilliary thing, it exposes hexadecimal serialization and deserialization,
since these are needed to display hashes anway.

[Documentation](https://docs.rs/bitcoin_hashes/)

## Minimum Supported Rust Version (MSRV)

This library should always compile with any combination of features on **Rust 1.29**.
However, due to some dependencies breaking their MSRV in patch releases, you may
need to pin these deps explicitly, e.g. with the following commands

```
cargo generate-lockfile
cargo update -p serde_json --precise "1.0.39"
```

## Contributions

Contributions are welcome, including additional hash function implementations.
