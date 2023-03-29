# mariadb_archive_server

## Setup
- [Install Rust](https://www.rust-lang.org/tools/install).
- run `'cargo run --release --'`

- To access the KB files, either clone [mariadb_archive](https://github.com/icerath/mariadb_archive) into the same directory as this repo, or run the [mariadb_crawler](https://github.com/icerath/mariadb_crawler).

Run with --help to see usage.

Keep it mind cargo might take a while for the first compile.

## Using the Server
- `localhost:[PORT]/kb/[url]` will respond with the original html and can be viewed like a regular webpage.
- `localhost:[PORT]/kb/[url]?list` will respond with all the subpages.
- `localhost:[PORT]/kb_urls.csv` will respond with the file's direct contents.
- `localhost:[PORT]/diff` will respond with the files missing from `kb_urls.csv`