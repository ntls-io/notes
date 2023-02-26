# choices

- Password hashing

  Looking at <https://github.com/ntls-io/ntls-sgx-service>,
  the password hashing algorithm used is __Argon2id__,
  which is the default (of the 3 variants) provided by [argon2 crate].
  See the OWASP [Password Storage Cheat Sheet] for what makes this a good choice.

- Data hashing

  Looking at <https://github.com/ntls-io/ntls-sgx-service>,
  the data hashing algorithm used is __BLAKE3__,
  which is chosen for [its speed].

- Data encryption

  Looking at <https://github.com/ntls-io/ntls-sgx-service>,
  the encryption algorithm chosen is __ChaCha20-Poly1305__,
  due to it being state-of-the-art.
  It is accessed through [ring_compat] crate.

[Password Storage Cheat Sheet]: https://cheatsheetseries.owasp.org/cheatsheets/Password_Storage_Cheat_Sheet
[argon2 crate]: https://lib.rs/crates/argon2
[its speed]: https://github.com/BLAKE3-team/BLAKE3
[ring_compat]: https://github.com/RustCrypto/ring-compat
