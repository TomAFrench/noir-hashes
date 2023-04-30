# Noir Hashes

Implementations of various hash functions in Noir.

## Hash functions in the Noir standard library

Some hash functions are implemented inside the [Noir standard library](https://github.com/noir-lang/noir/blob/master/noir_stdlib/src/hash.nr). This is because proving backends may implement optimized native versions of these hash functions. This allows these hash functions to be used with much fewer constraints than when implemented in pure Noir.

These hash functions are:

- sha256
- blake2s
- keccak256
- pedersen

Note that not all proving backends will have a native implementation of these hash functions and then will fallback to a Noir implementation.
