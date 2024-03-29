This code is archived here for historical purposes.

Downloaded from https://packetstormsecurity.com/files/21444/snuffle.shar.html

See: https://en.wikipedia.org/wiki/Bernstein_v._United_States

Snuffle has been superceded by Salsa20/Snuffle 2005: https://cr.yp.to/snuffle.html

Original usenet post:

> snuffle - generic hash-based encryption and decryption programs
>
> snuffle and unsnuffle turn any good one-way hash function (such as
> Merkle's Snefru) into a reasonably fast private-key encryption method.
> You must have Snefru, or something providing the same Hash512()
> interface, for snuffle and unsnuffle to work. Past that, snuffle and
> unsnuffle should be perfectly portable.
> 
> On this Sun 4, snuffle and unsnuffle encrypt between two and three times
> slower than crypt(1). However, they provide a lot more security.
> 
> snuffle is public domain. Send any comments to the newsgroup sci.crypt,
> which the author reads whenever possible. I do *not* know whether
> snuffle is legally exportable; it contains no encryption technology, but
> I'm not going to try sending it outside the United States.
> 
> Start by making symbolic links or copies of snefru's hash512.o,
> sboxes.o, snefru.h, and patchlevel.h in this directory. Then edit the
> options in the Makefile and compile. Read snuffle.man and you're off.
