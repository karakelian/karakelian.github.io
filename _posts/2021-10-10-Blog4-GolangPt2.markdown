---
layout: post
title:  "Blog 4 - Golang pt. 2"
date:   2021-10-10 5:15:29 -0700
categories: Tech
---
## Golang: Going In Depth
Last week, we reviewed how Go is a compiled programming language that is syntactically similar to C, but includes other various features such as structural typing, memory safety and etc. This week, we are going touch upon more complex designs and implementations that are possible with Go. We will touch upon its Package System, Concurrency (goroutines and channels), Binaries, and Omissions. To display its use in the industry, we will also provide real-world examples of applications that are written in Go. To start, let's review the package system in Go and find out the default path, names and references in its applications.

## Package Systems
Each package in Go's package system has a path and a name that might have references to other packages. These package definitions have to be prefixed with the name of the other package, and are case-sensitive. For example, if you are trying to reach the package system of the reader application, `io.Reader` would be the correct path because it is case-sensitive. If you try to find the package system by searching for `io.reader` or `bzip2.reader`, there will be no package systems returned. These package systems can be retrieved using the `go get` command. Developers that use go in applications promote the development of packages inside a base path which corresponds to the source repository. This is because the naming convention is less likely to cause collisions if the standard library or external libraries had future additions. As of recently, there have also been proposals to introduce proper package management.
<br/><br/>
Example Package System Path:
<br/>
`"compress/bzip2"`
<br/>
`"golang.org/x/net/html"`
<br/><br/>
<img src="https://www.callicoder.com/static/a5258526ae54e5c5e977c741d1bc2cfb/bd6b9/go-package-illustration.jpg" alt="MSC" width="460" height="345">

## Concurrency | Goroutines and Channels
Since Go has built-in facilities which allow for library support when writing concurrent programs, concurrency is a significant feature as it allows other processing to continue before the transmission has finished. In Go, the primary concurrency is labeled as the `goroutine`. The goroutine is essentially a light-weight process that will start a function with the `go` keywords. Most of the classical concurrency tools such as the mutex locks are available on the standard library, but idiomatic concurrency programs might require a different concurrency known as channels.
<br/><br/>
Channels are a typed concurrency in Go, in the sense that a channel of type `chan S` can only transfer messages to that of `type S`. For this reason, channels are important when special syntax is necessary to operate on them. The entire existence of channels in Go operate on the actor model-style, which are very similar to that of Erlang, where messages can be addressed to actors directly (similar to goroutines). Using these types of concurrencies, developers in Go can build concurrent constructs which include pipelines, worker pools, and etc. Channels can also be useful in interprocess communication, which would include applications like a concurrency-safe list of recycled buffers. 
<br/><br/>
<img src="https://res.cloudinary.com/practicaldev/image/fetch/s--bu0AUXp5--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://thepracticaldev.s3.amazonaws.com/i/xomfm3cx84cftpps3iq6.jpg" alt="MSC" width="460" height="345">

## Binaries and Omissions
Statically linked binaries are created by default with the linker in the gc toolchain. This means that all Go binaries are included with Go runtime. For this reason, Go deliberately will omit certain features that might be common in many other languages. Some of these examples include inheritance, pointer arithmetic, implicit type conversions, tagged unions, and etc. This is mainly because the designers of Go only included facilities that were mutually agreed upon. Throughout the various omitted features, the designers of Go also argued against pointer arithmetic and assertions because they wanted to encourage the use of interfaces. By utilizing interfaces, developers would also learn how to properly achieve dynamic dispatch to reuse code with their composition. As we will later mention, these omitted features can either be perceived by harsh criticism or a modern perspective on language features. It is important to note that Go designers express an openness to the generic programming of many languages, as they are still open to standardizing methods to apply code generation.

### Real World Applications
There are many notable open-source applications written in Go:
<br/>
- `Hugo`: The application that some of us have been using in this class to make our github website.
- `Kubernetes`: The container management system for which we had a two-part blog previously.
- `Dropbox`: The well known file hosting service.
- `Netflix`: The movie/show streaming service uses Go for two portions of their server architecture
- `Soundcloud`: The music streaming service utilizing Go for "dozens of systems"
- `Twitch`: The user streaming service applies Go for their IRC-based chat system.
<br/><br/>
<img src="https://miro.medium.com/max/1400/1*H2gxU4Ha2Ie2X-e4QWo66w.jpeg" alt="MSC" width="460" height="345">


## Criticisms
Although our last blog touched upon some common criticisms, these are remarks that Go critics have noted for developers that have been using Go as their primary language in real world applications. 
<br/>
Due to Go's lack of algebraic types, many developers note that this leads to difficulty in handling failures and debugging base cases. There are also remarks made to how Go does not allow an opening brace to appear on a line of its own, which makes programmers use the same brace style. Although these two criticisms are specific, they are very common with developers that use the language very often, and have become tedious issues. Another noteworthy criticism is that file semantics in Go are heavily based on POSIX semantics. This means that most of the semantics will not map well to the Windows platform. A recent remark in Go forums have also noted that it is easy to make concurrency bugs due to message parsing within shared memory. To find out more noteworthy issues, visit [Toptal][critic-io]


### Golang Help
You can visit [Golang][golang-io] to access documents, packages and example projects coded in Go., and learn more about the fundamentals of Go, research specific documentation. Like any programming community, Go offers wide support through their Go [Forum][forum-io]. This gives users access to their Discord, Slack, and IRC Channels, along with other features that can better help and assist in your learning with the programming language. 
<br/><br/>
Stay tuned for a new blog topic next week!

[golang-io]: https://golang.org/
[forum-io]: https://golang.org/help 
[critic-io]: https://www.toptal.com/go/4-go-language-criticisms 