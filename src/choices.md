# choices

- Password hasing

  Looking at <https://github.com/ntls-io/ntls-sgx-service>,
  the password hashing algorithm used is __Argon2id__,
  which is the default (of the 3 variants) provided by [argon2 crate].
  See the OWASP [Password Storage Cheat Sheet] for what makes this is a good choice.

  _See [mdBook docs] for details on how it works_
  
[Password Storage Cheat Sheet]: https://cheatsheetseries.owasp.org/cheatsheets/Password_Storage_Cheat_Sheet
[argon2 crate]: https://lib.rs/crates/argon2

