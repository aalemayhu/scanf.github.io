---
layout: post
title: compiling linux part 2
---


Feeling sick again, I decided to compile the kernel with the same configuration
but did some research on how to speed it up and as usual landed on SO.  Reading
this
[post](http://stackoverflow.com/questions/23279178/how-to-speed-up-linux-kernel-compilation)
I tried `make ARCH=x86_64 -j4` which was faster and the output of `time` was:

    real    17m56.588s
    user    69m21.700s
    sys     3m41.752s

I used commit
[d19d133e432248c9b3efa9c10dda5f050cbbcd72](https://github.com/torvalds/linux/commit/d19d133e432248c9b3efa9c10dda5f050cbbcd72).

