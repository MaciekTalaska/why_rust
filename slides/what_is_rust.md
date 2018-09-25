## What is Rust
====


### Rust is:

* system language
* compiles to native code (no VM)
* no automatic memory management (gc)
* no implicit boxing
* syntax inspired by C/C++
* rustc uses LLVM as a backend
* macros
====


### What is system language?

* may operate on lower level of abstraction
* used to build building blocks for others
* efficiency/little overhead
* inlining assembly
* good for creating drivers, parts of OS
====


### Rust IS system language

* Redox (https://www.redox-os.org/)
* intermezzOS (https://intermezzos.github.io/)

Note:
* Redox = Unix like OS
* intermezzOS = OS creating for learning purposes (book on OS develpment is available)
====


### Rust concurrency

* threads
* message passing
* shared state concurrency
* extensible concurrency
* more: http://www.yetanother.site/rust-cookbook/concurrency.html
* async?: tokyo! (https://github.com/tokio-rs/tokio)
* use/search for crates!

Note:
* extensible concurrency: use Send/Sync traits 
====


### Wide platform support

* Tier 1
* Tier 2
* Tier 2.5
* Tier 3

<small>(source: https://forge.rust-lang.org/platform-support.html)</small>

Note:
* t1: official build, automatic tests, documentation on how to build/use
* t2: official build, automatic build (but may lack tests), features include because it builds, not because tests passed (as for t1)
* t2.5: build not avail. via rustup, rest same as for t2
* t3: supported, but are not built/tested automatically. May not work. No official builds.
====


### Tier 1 (guaranteed to work)

* OSX (10.7) 32bit/64bit
* Windows (7+) 32bit/64bit
* Linux 32bit/64bit

Note:
* Windows in 2 flavors: MSVC & GNU
* official build, automatic tests, documentation on how to build/use
====


### Tier 2 (guaranteed to build)

* Arch64: iOS, Android, Fuchsia, Linux
* Arm7: iOS, Linux, Android
* i686: FreeBSD, Linux
* mips, mips64, mipsel
* sparcv9, sparc64, powerpc, powerpc64
* wasm32

Note:
t2: official build, automatic build (but may lack tests), features include because it builds, not because tests passed (as for t1)
====


### Tier 2.5 (guaranteed to build)

**accidental status**
* aarch64-unknown-cloudabi
* armv7-unknown-cloudabi-eabihf
* i686-unknown-cloudabi
* powerpc-unknown-linux-gnuspe
* sparc-unknown-linux-gnu

Note: 
* no new platforms should reach this state!
* build not avail. via rustup, rest same as for t2
====


### Tier 3 

* Haiku 32/64
* Windows XP 32/64
* NetBSD
* NaCl
* DragonFly 64bit
* NVPTX

Note:
t3: supported, but are not built/tested automatically. May not work. No official builds.
