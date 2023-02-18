To build these docs,
install __mdBook__ from [its download page]
(unless you have a recent Rust toolchain, in which case you would just `cargo install mdbook`),
and run this command:

```
mdbook serve --open
````

Above command will (conveniently) open the documentation in a web browser.

_See [mdBook docs] for more detail on how it works._

---

Following are additional (and optional) executables to install:

- `mdbook-mermaid` for displaying [Mermaid diagrams]
  ([download page][mermaid-download-page])
- `mdbook-toc` for displaying table of contents on individual chapters
  ([download page][toc-download-page])
- `mdbook-admonish` for displaying pretty side content
  ([download page][admonish-download-page])

[its download page]: https://github.com/rust-lang/mdBook/releases/latest
[mdBook docs]: https://rust-lang.github.io/mdBook
[Mermaid diagrams]: https://mermaid.js.org
[mermaid-download-page]: https://github.com/badboy/mdbook-mermaid/releases/latest
[toc-download-page]: https://github.com/badboy/mdbook-toc/releases/latest
[admonish-download-page]: https://github.com/tommilligan/mdbook-admonish/releases/latest
