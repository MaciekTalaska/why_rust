## Disadvantages of Rust
====


### Hard to learn

* "I can't pass string as argument!"
* borrow/checker
* "value already moved"

Note:
* Rust aims at competing with C++ and is C++ easy to learn?
* Would you master C++ in a half a year? A year? And Rust?
====


### Rust is more low level than Java/C#/Clojure etc.

* development speed (Java/C#/TypeScript)
 * cost of the software
* is it good for solving **business** problems?

Note:
* same as with C++: business apps are not written in C++ anymore
* for webapps databse/network is bottleneck, you won't get much improvement just from using "fast" language (why is/was YouTube written in Python?)
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
* debugging symbols for debug & release 
* compilator options (Cargo.toml)

Note:
* you may use strip to get rid of symbols
* UPX greatly reduces size of Rust binaries (down to ~50%)
====


### There is no perfect/ideal language!

* it is interesting, but:
 * it was inspired by many other languages
 * there were some languages trying to solve the problem in the past
 * fp addresses concurrency
* **do not** be a Rust fanatic!
====

### Take-away:

* multithreading
* memory-safety (data-races)
* wide platform support
* raw performance
* great tooling, great documentation, great support
* FUN!
