# ltl-layout-engine

> Flexbox-inspired 2-D layout engine with min/max sizing.

Written in **[Lateralus](https://lateralus.dev)** — a statically typed,
pipeline-oriented programming language.

## Quick start

```bash
# install the lateralus toolchain (one-liner)
curl -sSL https://lateralus.dev/install.sh | sh

# clone and build
git clone https://github.com/bad-antics/ltl-layout-engine.git
cd ltl-layout-engine
lateralus run main.ltl
```

## What's inside

```
.
├── .gitattributes
├── LICENSE
├── README.md
└── main.ltl
```

See [`main.ltl`](main.ltl) for the entry point.

## Why Lateralus?

Lateralus compiles straight to C99, LLVM IR, JavaScript, and WebAssembly,
so a tool written in it runs anywhere those targets run. The pipeline
operator (`|>`) makes data-flow code read top-to-bottom:

```lateralus
let result = input
    |> parse
    |> transform
    |> filter(|x| x.is_valid())
    |> collect_into_list()
```

## License

MIT. See [LICENSE](LICENSE).

## Related

- **Main language repository**: [bad-antics/lateralus-lang](https://github.com/bad-antics/lateralus-lang)
- **Standard library**: [bad-antics/lateralus-stdlib](https://github.com/bad-antics/lateralus-stdlib)
- **Documentation**: [lateralus.dev](https://lateralus.dev)
