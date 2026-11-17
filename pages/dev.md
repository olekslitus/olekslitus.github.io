---
layout: page
title: /dev
permalink: /dev/
---

# /dev

### apps
- [lines](https://olekslitus.com/lines/) - calm, beautiful notes that stay yours

### teaching
- Helped design and TAed DS3500 with Prof. Rachlin

### written in C
- [nush](https://github.com/olekslitus/nush) - shell with support for pipes and variables
- [xmalloc](https://github.com/olekslitus/xmalloc) - super-fast thread-safe memmory allocator
- [olfs](https://github.com/olekslitus/olfs) - performent unlimited nesting file system based on [Linux FUSE](https://www.kernel.org/doc/html/latest/filesystems/fuse.html)

### i help with ...
- [tui-rs](https://github.com/fdehau/tui-rs) - terminal user interfaces and dashboards using Rust

### reads
- [fst](https://blog.burntsushi.net/transducers/) like trie, but better
- [trie](https://medium.com/shyft-network-media/understanding-trie-databases-in-ethereum-9f03d2c3325d) in eth

### ideas
- leximoron - programming languages database
- oleks.studio - design studio


```racket
(define Y (λ (b) ((λ (f) (b (λ (x) ((f f) x))))
                  (λ (f) (b (λ (x) ((f f) x)))))))
```
