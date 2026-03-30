# vinofyi

[![crates.io](https://img.shields.io/crates/v/vinofyi.svg)](https://crates.io/crates/vinofyi)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Wine encyclopedia with grapes, regions, and food pairings — API client for [vinofyi.com](https://vinofyi.com).

> **Try the interactive tools at [vinofyi.com](https://vinofyi.com)**

## Install

`cargo add vinofyi`

## Quick Start

```rust
use vinofyi::Client;

#[tokio::main]
async fn main() -> Result<(), Box<dyn std::error::Error>> {
    let client = Client::new();
    let result = client.search("cabernet-sauvignon").await?;
    println!("{} results", result.total);
    Ok(())
}
```

## Also Available

| Platform | Package | Link |
|----------|---------|------|
| **Python** | `pip install vinofyi` | [PyPI](https://pypi.org/project/vinofyi/) |
| **npm** | `npm install vinofyi` | [npm](https://www.npmjs.com/package/vinofyi) |
| **Go** | `go get github.com/fyipedia/vinofyi-go` | [pkg.go.dev](https://pkg.go.dev/github.com/fyipedia/vinofyi-go) |
| **Rust** | `cargo add vinofyi` | [crates.io](https://crates.io/crates/vinofyi) |
| **Ruby** | `gem install vinofyi` | [rubygems](https://rubygems.org/gems/vinofyi) |

## Embed Widget

Embed [VinoFYI](https://vinofyi.com) widgets on any website with [vinofyi-embed](https://widget.vinofyi.com):

```html
<script src="https://cdn.jsdelivr.net/npm/vinofyi-embed@1/dist/embed.min.js"></script>
<div data-vinofyi="entity" data-slug="cabernet-sauvignon"></div>
```

Zero dependencies · Shadow DOM · 4 themes (light/dark/sepia/auto) · [Widget docs](https://widget.vinofyi.com)

## Links

- [VinoFYI](https://vinofyi.com) — Main site
- [API Documentation](https://vinofyi.com/developers/)
- [OpenAPI Spec](https://vinofyi.com/api/openapi.json)
- [Glossary](https://vinofyi.com/glossary/)

## License

MIT
