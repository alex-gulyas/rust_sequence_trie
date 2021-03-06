[Sequence Trie][doc]
====

[![Build Status](https://travis-ci.org/michaelsproul/rust_sequence_trie.svg)](https://travis-ci.org/michaelsproul/rust_sequence_trie)

This is a generic Trie implementation that uses a hash map to store child nodes. The Trie is keyed by lists of type `K`, which can be anything implementing `PartialEq`, `Eq`, `Hash` and `Clone`. If your keys are explicit lists and you want to be able to store a different value for each fragment of a key, this might be the data structure for you!

I'm still undecided about what to call this data-structure, as it's kind of half-way between an unbounded tree and a trie... Suggestions welcome.

For more information, see the [documentation][doc].

[doc]: https://michaelsproul.github.io/rust_sequence_trie/

# Usage

Add `sequence_trie` to your `Cargo.toml`.

```toml
[dependencies]
sequence_trie = "*"
```

# See Also

Since writing this sequence trie I've created a radix trie which uses node compression. It has *much* better performance and has reached feature-parity.

https://github.com/michaelsproul/rust_radix_trie

# License

MIT License. Copyright (c) Michael Sproul 2015.
