# problems

- When compiling a Teaclave project,
  you may counter an error similar to the following:

  ```
  > error[E0152]: duplicate lang item in crate `std`: `panic_impl`.
    |
    = note: the lang item is first defined in crate `sgx_tstd` (which `counter` depends on)
    = note: first definition in `sgx_tstd` loaded from /home/tshepang/work/ntls-enclaves/dataset-hashing/enclave/target/debug/deps/libsgx_tstd-6cdbb9551fc70463.rmeta
    = note: second definition in `std` loaded from /home/tshepang/.rustup/toolchains/nightly-2022-10-22-x86_64-unknown-linux-gnu/lib/rustlib/x86_64-unknown-linux-gnu/lib/libstd-7b2106000b625742.rlib
  ```

  A likely cause could be using a crate that has `std` enabled,
  which conflicts with the `std` crate of Teaclave.
  Avoid it by disabling that `std` feature of that crate.
  An example of doing so is running the following command,
  which uses `blake3` as an example:

  ```
  cargo add blake3 --no-default-features
  ````
