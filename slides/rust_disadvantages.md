## Disadvantages of Rust
====


### Hard to learn

* "I can't pass string as argument!"
* borrow/checker
* "value already moved"

Note:
* Rust aims at competing with C++ and is C++ easy to learn?
====


### Rust is more low level than Java/C#/Clojure etc.

* development speed (Java/C#/TypeScript)
 * cost of the software
* is it good for solving **business** problems?

Note:

====


### Is still in development

* example: (benchmarking not on stable)
* huge binaries ('-z' is already in)
* why discussions take so long in Rust community?

Note:
* Rust community decided it's better to think carefully of introducing a feature, before including it, than to remove it aftwerwards and break backward compatibility
====


### Rust binary size

By default Rust image is pretty big
(and grows fast)

* static linking of standard library
* debugging symbols
* compilator options (Cargo.toml)
====


### Rust is not the greatest language of all times!

* it is interesting, but:
 * it was inspired by many other languages
 * there were some languages trying to solve the problem in the past
 * fp addresses concurrency
* **do not** be a Rust fanatic!
