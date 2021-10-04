---
layout: post
title:  "Blog 3 - Golang"
date:   2021-10-03 3:15:29 -0700
categories: Tech
---
## Golang: The Programming Language
Go is a compiled programming language that is statically typed and designed at Google. This language is syntactically similar to C, but includes other various features such as structural typing, memory safety and etc. Although the programming language is named `Go`, it is often referred to as `Golang` because of its domain name `goland.org`. Before we jump into learning more about this programming language, it is important to note that there are two major implementations of Go. The first is Google's self-hosting toolchain which targets various O.S.'s along with WebAssembly. The second implementation is gofrontend, which is a frontend used for other compilers. In this blog, we are going to go the Design, Style and Tools within Golang, and provide examples using the programming language itself. Let's jump right into the Design of Go!
<br/><br/>
<img src="https://miro.medium.com/max/2000/1*8bPiDNL1K1ZdK9O_T5IVKw.png" alt="MSC" width="460" height="345">

## Go: Design
Since Go is influenced primarily by the programming language `C`, the language consists of many similarities such as a syntax environment, fast compilation, and remote package management. There are also different approaches to problem solving which include built-in concurrency primitives. These refer to channels, light-weight processes and the select statement (which we will touch upon later). The interface of Go also utilizes virtual inheritance, type embedding and a toolchain which produces statically linked native binaries by default. Golang also likes to keep the language specification simple by removing features that are common in similar languages, to reduce cross confusion. The main part of Golang's design is its syntax, which includes changes from C. The syntax in Go is aimed to keep code readable and concise by introducing combined declarations and initialization operators. 
<br/><br/>
This allows programmers to write commands such as `i :=3 ` and `s := "Hello, world!" ` without specifying variable types. In other languages such as C, the same commands would be written as `int i = 3 ` and `const char *s = "Hello, world!"`, where variable types are stated. Go also includes return values by employing commands such as `result, err`. 

## Go: Style
The programmers that created Go but significant effort in influencing the style of programs in Go, which include surface-level details such as indentation, spacing and additional automatic style checks. Other tools and libraries focus on API documentation such as `gocdoc`, which include testing, building, and package management through `go test`, `go build` and `go get`. Furthermore, Go is set to enforce rules that would otherwise be recommendations in certain programming languages. Examples of this style type include banning cyclic dependencies, imports, implicitly type conversions and unused variables. Removing features that are also apparent in other programming language such as `map` and `try` also encourage programmers to stick to a more particular and concrete programming style. The first day Go was released, the Go team also published a set of `Go Idioms` which are essentially blogs and reviews on how to teach Go style and apply their coding philosophy.

### Tools In Go 
- `go build`: Build  is used to build Go binaries using information in solely the source files, and no seperate makefules
- `go test`: Test is used for unit testing and setting microbenchmarks
- `go fmt`: Fmt is for formatting code
- `go install`: Install is used to install and retrieve remote packages
- `go vet`: Vet is a static analyzer which looks for any errors in the code
- `go run`: Run is a shortcut which builds and executes code
<br/>
Other tools that are not as commonly used are `godoc`, `gorename` and `go generate`, which display documentation, rename variables and invoke code generators respectively
<img src="https://www.tutorialandexample.com/wp-content/uploads/2021/02/Tools-for-GoLang.png" alt="MSC" width="460" height="345">

## Golang | Common Criticisms
Just like any other programming language, Golang is subject to criticism of its own. The first main criticism that many users have issues with is the lack of function overloading an default values for arguments. Since GO doesn't provide passing default values for overloaded functions, users often have to write their code in a specific way to get around this. For this example, take the code that would be employed in Go: `func (wd *remoteWD) WaitWithTimeoutAndInterval(condition Condition, timeout, interval time.Duration) error {`. The implementation in this code differs if it were to be coded in a language like JavaScript: `function Wait (condition, timeout = DefaultWaitTimeout, interval = DefaultWaitInterval) {` Here the values are passed by default to a function that may or may not be overloaded.
<br/><br/>
Another criticism of Go are the lack of generics. This refers to a situation where programmers may want to write a map function, as Go does not support function overloading and will require multiple implementations with different function names.  Dependency Management is another common issue in Go because of version management. This issue arises when library maintainers makes incompatible changes and uploads it to github, which will give an error to any user to tries to use the program after. This is because `go get` is essentially the same as `git clone`. Without installing the library files, the program will not compile. 
## Coding In Go
Coding in Go may be different to users that are set with similar syntax in languages such as C++, C, or Java, but the process is very much the same. In this code below, take a look at the setup of the main block of code, along with calling the function main. The function for `say` performs a `for loop` that will run until the iterator reaches a value of 5, and print out the word hello. Notice the use of the `go fmt` tool that we just reviewed as well!

<br/>
<img src="https://i.stack.imgur.com/dTxVq.jpg" alt="MSC" width="600" height="345">
<br/><br/>

This last example of code below also shows the import of the `go fmt` tool, along with a function called `whatdayisit` that will print output based on the date/time.
<img src="https://miro.medium.com/max/1400/1*1SVdQfxQ3Ku3iHpSswm9rw.png" alt="MSC" width="600" height="345">

### Learn More About Golang
To learn more about the programming language Go, visit [Golang][golang-io] to access documents, packages and example projects coded in Go. You can learn more about the fundamentals of Go, research specific documentation, and get in touch with teams of users. Just like any programming community, Go offers wide support through their Go [Forum][forum-io]. This gives users access to their Discord, Slack, and IRC Channels, along with other features that can better help and assist in your learning with the programming language. 
<br/><br/>
Stay tuned for a new blog next week!

[golang-io]: https://golang.org/
[forum-io]: https://golang.org/help 
