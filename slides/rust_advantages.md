## Rust is good for... 
====


### calculation intensitive tasks

* in pair with C
* in pair with C++
* faster then Go
* faster than Java

more info: https://benchmarksgame-team.pages.debian.net/benchmarksgame/
====


### embedded programming

* does not require runtime
* wide support for platforms (arm!)
* no additional memory overhead
====


### web programming (webassembly)

* smaller amount of data to transfer
* computationaly intensive tasks
* performance oriented tasks for networking (Go niche)
====


### Game development

Rust is slowly getting some attention from game industry

* performace comparable to C/C++
* addresses problems of data races
* http://arewegameyet.com/
* https://www.youtube.com/watch?v=P9u8x13W7UE
====


## Demoscene

<iframe width="1175" height="661" src="https://www.youtube.com/embed/rWwNgVwQG1A" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

====


### Native gems/eggs

* Python/Ruby are popular but very slow
* both suffer from GIL problem
* Rust for the rescue?

Note:
* Rust is good not only for raw performance (in pair with C/C++)
* Rust is also good for writing multithreaded code (for each CPU produced after ~2006-2008)
====


### CLI tools

* no dependencies
* relatively small (could be optimized)
* offers good performance
* some tasks that are CPU intensive

Note:
* size optimization could be made in Cargo.toml, or by... UPX
* intensive tasks: calc file hash, packing/unpacking files, archive integrity, par2 file integrity checks etc. 
====

### Who uses Rust?

1aim, 360dialog, 49nord, 3DR, Academia.edu, AgilData, AISenz, Algorithmia, **ANIXE**, AppSignal, Ather Energy, **Atlassian**, Autumn, Beget, BePark, Braintree, Calyptech, Cambridge Consultants, **Canonical**, **Ceph**, Chef, Clever Cloud, Cloudflare, CodePicnic, **Coursera**, Coredump Hackerspace, Coturnix, craft ai, Cultivate Software, Dazta, Delimiter, Deliveroo, **Dropbox**, ETCDEV Team, **Parity Technologies**, Everlane, Faraday, Fortanix, GiGa infosystems GmbH, Gremlin Inc, Habitat, Honeypot, ImageOptim, krypt.co, kupibilet.ru, LINE, Linkerd, Linki Tools, MaidSafe, **Mozilla**, Navitia, **npm**, Inc, Omnijar Studio, OneSignal, **OVH**, Pants Build, Pollen Robotics, Postlight, Postmates, PingCAP, PurchaseClinic.com, QCERT (Qatar's National CERT), Sandstorm, Scality, Sentry, slowtec, SmartThings, Snapview, Snips, Spoqa, Stratum Security, superscale networks, System76, Telenor Digital, Tessel, thoughtram, ThreatX, Threema, Tilde, TrafficLand, Wire, Xero, AdHawk, TreeScale, EVO.company, PolySync, Cryptape, **CoreOS**, Inc., 3D Hubs, VersionEye, VOYAGE GROUP, Angelcam, tCell, Structure Systems, 10x Genomics, 1300 Web Pro, Wildfish, Bitfury Group, WINK Streaming, Collective Sense, Shiftleft, Tocco AG, Pressjitsu Inc, Baidu X-Lab, CurrySoftware GmbH, Schauspiel Dortmund, Centricular, Galois, Metaswitch, Nomalab, CancerIQ, IamBot, HealPay, Zeplin, Starry, Tonsser, Tula Technology, ChartMogul, FacturaDirecta, Yomura Fiber, NAVITAS Solutions GmbH, Webbula, Imeka, Figma, EXSigma, Sourcegraph, Aprila Bank, Fire and Emergency NZ, Solana, Kodebox, TenX, Star Lab

https://www.rust-lang.org/en-US/friends.html
