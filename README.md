# go-toml V2

Development branch. Probably does not work.

[👉 Discussion on github](https://github.com/pelletier/go-toml/discussions/471).

## Must do

- [x] Unmarshal into maps.
- [x] Support Array Tables.
- [x] Unmarshal into pointers.
- [x] Support Date / times.
- [x] Support struct tags annotations.
- [x] Support Arrays.
- [x] Support Unmarshaler interface.
- [x] Original go-toml unmarshal tests pass.
- [x] Benchmark!
- [x] Abstract AST.
- [ ] Original go-toml testgen tests pass.
- [ ] Attach comments to AST (gated by parser flag).
- [ ] Track file position (line, column) for errors.
- [ ] Benchmark again!

## Further work

- [x] Rewrite AST to use a single array as storage instead of one allocation per
      node.
- [ ] Provide "minimal allocations" option that uses `unsafe` to reuse the input
      byte array as storage for strings.
- [x] Cache reflection operations per type.

## Ideas

- [ ] Allow types to implement a `ASTUnmarshaler` interface to unmarshal
      straight from the AST?

## License

The MIT License (MIT). Read [LICENSE](LICENSE).
