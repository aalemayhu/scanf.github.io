---
layout: post
title: Productivity and Go 
---

After being inspired by [David
Allen](https://www.youtube.com/watch?v=Qo7vUdKTlhk), I've been extensively
tracking things in Google Keep. So whenever I think about something, and am
convinced that it is very important, I try to pull up my Nexus and make a note.
I'd like to think that I have been less stressed out, but it's hard to say
without actually measuring it.

I attended [Fosdem](https://fosdem.org/2015/) in January and it was awesome. I
made a scheduel before traveling to Brussel, but ended up spending most of my
time in the Go devroom. I naturally got more into Go. In the last couple of
days I've just been reading random code in the project. I keep finding
interesting ways to contribute, thanks to the Go authors for adding their
`TODO` notes throughout the project. Maybe I can contribute soon? The only
things blocking me currently are:

1. The syntax is still too new for me.

   While I really enjoy writing Go and it's just pure fun. I really feel the
   lack of a firm grip in the language. I think this will probably be resolved,
   after I am trough with the [tour.golang.org](http://tour.golang.org/) and
   have read [The Go Programming Language
   Specification](https://golang.org/ref/spec). The primary reason it's taking
   so long is; I keep looking up the stuff mentioned in the tour, currently I
   am reading the source for the [`time`](http://golang.org/src/time/) package.

2. The Go authors have a process for contributing.

   In order to avoid duplicate work, you let people know what you are working
   on. Before writing code ideally you should discuss your design. After writing
   some code, you submit it to gerrit for review and just wait. While I have
   not gone through this process reading about it in the [Contribution
   Guidelines](https://golang.org/doc/contribute.html) does seem to give a
   general picture for new contributors. Will try to reread it again in the
   future.

So what would I do if I could change something today? Well I think implementing
`execve` would be a good start. I wonder if it would be fun? There are also
other system calls for linux that are not implemented in the
[`syscall`](http://golang.org/src/syscall/syscall_linux.go) package.
