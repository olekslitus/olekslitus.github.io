---
layout: page
title: /dev
permalink: /dev/
---

# /dev


---
```racket
(define Y (λ (b) ((λ (f) (b (λ (x) ((f f) x))))
                  (λ (f) (b (λ (x) ((f f) x)))))))
```
---
