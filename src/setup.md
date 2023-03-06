To build these docs,
install __mdBook__ from [its download page]
(unless you have a recent Rust toolchain, in which case you would just `cargo install mdbook`),
and run this command:

```
mdbook serve --open
````

Above command will (conveniently) open the documentation in a web browser.

_See [mdBook docs] for more detail on how it works._

#### optional dependencies

Following are additional (and optional) executables to install:

- `mdbook-mermaid` for displaying [Mermaid diagrams]
  ([download page][mermaid-download-page])
- `mdbook-toc` for displaying table of contents on individual chapters
  ([download page][toc-download-page])
- `mdbook-admonish` for displaying pretty side content
  ([download page][admonish-download-page])


#### licenses

This project is under MIT License,
and a copy is included at the root of the repository.

Dependencies:

- [Mermaid is under MIT license], and so are its bundled assets,
  [mermaid.min.js](assets/mermaid.min.js).
- [mdbook-admonish is under MIT license], and so are its bundled assets,
  [mdbook-admonish.css](assets/mdbook-admonish.css)
- [mdbook-toc is under MPL license]

[its download page]: https://github.com/rust-lang/mdBook/releases/latest
[mdBook docs]: https://rust-lang.github.io/mdBook
[Mermaid diagrams]: https://mermaid.js.org
[mermaid-download-page]: https://github.com/badboy/mdbook-mermaid/releases/latest
[toc-download-page]: https://github.com/badboy/mdbook-toc/releases/latest
[admonish-download-page]: https://github.com/tommilligan/mdbook-admonish/releases/latest
[Mermaid is under MIT license]: https://github.com/knsv/mermaid/blob/master/LICENSE
[mermaid.min.js]: assets/mermaid.min.js
[mdbook-toc is under MPL license]: https://github.com/badboy/mdbook-toc/blob/main/LICENSE
[mdbook-admonish is under MIT license]: https://github.com/tommilligan/mdbook-admonish/blob/main/LICENSE
