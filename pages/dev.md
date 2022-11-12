---
layout: page
title: /dev
permalink: /dev/
---

# /dev

### teaching
- Helped design and TAed DS3500 with Prof. Rachlin

### written in C
- [nush](https://github.com/oreksu/nush) - shell with support for pipes and variables
- [xmalloc](https://github.com/oreksu/xmalloc) - super-fast thread-safe memmory allocator
- [olfs](https://github.com/oreksu/olfs) - performent unlimited nesting file system based on [Linux FUSE](https://www.kernel.org/doc/html/latest/filesystems/fuse.html)

### cli apps
- [dih](https://github.com/oreksu/dih) - do i have ...?
- [lit](https://github.com/oreksu/lit) - lighter git

### i help with ...
- [tui-rs](https://github.com/fdehau/tui-rs) - terminal user interfaces and dashboards using Rust

### reads
- [fst](https://blog.burntsushi.net/transducers/) like trie, but better
- [trie](https://medium.com/shyft-network-media/understanding-trie-databases-in-ethereum-9f03d2c3325d) in eth

### ideas
- [leximoron]() - programming languages database
- [oleks.studio](https://oleks.studio) - design studio


```racket
(define Y (λ (b) ((λ (f) (b (λ (x) ((f f) x))))
                  (λ (f) (b (λ (x) ((f f) x)))))))
```
