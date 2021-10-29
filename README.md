{{#title 電算部}}

# ここについて

このリポジトリは電算部のリポジトリです

# セットアップ方法

1. [Rust](https://www.rust-lang.org/ja/tools/install)からインストーラーをダウンロードします。
2. インストーラーを実行すると、標準ではパスが通ります。
3. コマンドプロンプトからmdbookをインストールします。

```shell
cargo install mdbook
```

4. リポジトリのルートディレクトリで、mdbookを起動します。

```shell
mdbook serve
```

5. 標準だと、

```url
http://localhost:3000
```

で立ち上がります。

# 使用したものについて

- [mdBook](https://github.com/rust-lang/mdBook)はrustで作られた文章管理ツールです。
- peaceiris様が作られた、[actions-mdbook](https://github.com/peaceiris/actions-mdbook)を使用しています。

# 書き方

Rustは実行できます。

```rust:editable
fn main() {
    println!("Hello, 電算部!");
}
```

MathJaxの数式も書けます。
\\[\int \int f(x,y) dx dy \\]
