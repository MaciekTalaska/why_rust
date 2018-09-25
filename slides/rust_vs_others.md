## Rust vs other languages
====

### Popularity of C++, C, Go, Rust 

![C++, C, Go, Rust](slides/c_cpp_go_rust_popularity.png)

(source: Google trends)
====


### Popularity of Go & Rust

![Go, Rust popularity](slides/go_rust_popularity.png)

(source: Google trends)
====


### Tiobe index (2017)

| No. | Language |
| ---: | :---: |
| 1. | Java |
| 2. | C |
| 3. | Python |
| 4. | C++ |
| 5. | VB.NET |
| 6. | C# |

https://www.tiobe.com/tiobe-index/
====


### Tiobe index (2017)

| No. | Language |
| ---: | :---: |
| 8. | Javascript |
| 14. | Assembly |
| 16. | Go |
| 22. | Dart |
| 25. | F# |
| 27. | Scala |
| 31. | Rust |


Note:
Rust is 31, but jumped from 36th places in 2016
====


### StackOverflow questions for C++, C, Go, Rust:

| Language | Questions |
| :---: | ---: |
| C++ | 585.811 |
| C | 284.890 |
| Go | 32.240 |
| Rust | 10.045  |

Note:
* as of 2018-09-20
* lots of question about libraries
* more question = language is more complicated?
====


### Rust vs Go. Similarities:

* both are "new"
* compile to native binaries 
* cross compilation
* address concurrency/multithreading

Note:
Go: 2009; Rust: 2015
====


### Rust vs Go. Differences:

|   | Go | Rust|
| --- | --- | --- |
| vm | no(?) | no |
| gc | yes | no |
| type classes/generics | no/yes | yes|
<br>
* Golang copes well with huge heaps
* Rust code is harder to read
* different niches

Note:
* Go is easier to understand for new programmers (even if they don't know Go at all)
* gc: JVM < 100ms, GO < 1m (but it is due to GO being so much different than Java)
* Go huge heaps: 18 GB and bigger (https://blog.golang.org/ismmkeynote)
* Go max stack size is 1 GB for 64bit, 250mb for 32bit
* source for last two: https://go101.org/article/memory-block.html
* biotech (bioinformatic), 300GB of data, breaking 512GB barieer of memory allocation for go: https://github.com/golang/go/issues/10460
====


### Rust vs Go: Concurrency is not parallelism

[![Concurrency is not parallelism](https://i.vimeocdn.com/video/343013570.jpg)](https://vimeo.com/49718712)

Note:
* Rust book simplifies, and assumes that concurrency=parallelism
* more info: http://tutorials.jenkov.com/java-concurrency/concurrency-vs-parallelism.html
* after (https://www.quora.com/What-is-the-difference-between-concurrency-and-parallelism/answer/Humoyun-Ahmedov): 
  * concurrency = be in progress simulatenously. it is design property!
  * parallelism = execute simulatenously. it is run-time property!
====


### Rust vs Cpp. C++ disadvantages:

- complicated
- metaprogramming
- preprocessor
- many keywords: 60+ (and new are added: ~90 now)
- keyword may have different meaning
- inconsistent standard library
- bad design decisions in the past (multi-inheritance)
- compilers are not compatbile
- slow development of C++
- long time for standard to be adopted

Note:
* different meanings: static (linkage, shortage etc.)
====


### Rust vs Cpp. C++ advantages:

- huge codebase
- a lot of resources
- popularity
- lots of libraries, tools
- huge pool of candidates / huge market
- defacto standard in some areas (gamedev, embedded, ML)
====


### Rust vs dynamic languages

* Perl, PHP, Python, Ruby...
* different niche
  * scripting in Rust?
  * web servers or web apps?
  * utilities
* desktop apps? 

Note:
* Rust has no dependency on runtime
* Rust is not great choice for business type apps
====


### Rust vs functional languages

* Rust is **NOT functional**
* has some functional inspired features:
   - map, fold, match etc.
* types are more "low-level"
* performance!
* no tail-call optimization
* impossible not to mutate state

Note:
* "impossible not to mutate" - sometimes this is how API works (rand)
* "functional": (Graydon): "Tail calls "play badly" with deterministic destruction. Including deterministic drop of ~ boxes. Not to say that they're not composable, but the options for composing them are UI-awkward, performance-penalizing, semantics-complicating or all of the above."
* https://github.com/rust-lang/rfcs/issues/271 - TCO is postponed, but "become" keyword has already been reserved for it
====


### Rust vs CLR/JVM languages

* runtime required
* higher abstraction
* Gc and overhead
* huge popularity, high adoption
* very good support (libraries)
* VM advantages:
 * GraalVM + Truffle
 * VM optimizations for future processors
 * new CPU feature = change Rust compiler, recompile Rust code
 * VM optimizes for different CPUs
====


### Rust vs D

* community
* perception
* no killer feature
* clear development path

Note:
* D seem to be "just better C++"
* it is hard to predict right now what are future plans for D
* D was shortly used at Facebook
* D standard library v1 was abandoned
* D should be compared to C++ than Rust 
====


### Rust vs Exotic languages:

 - Nim (Nimrod)
 - Julia
 - Crystal
 - Swift

Note:
1. Nim = "Python with GC and compiling to native code/c/c++/js"
2. Julia: gc, dynamic - for numerical analysis, computational science
3. Crystal: "native ruby", no parallelism (but has green threads); Problems on Windows
4. Swift: inspired by C#, replacement for ObjectiveC, mostly for mobile development, not a system language (
