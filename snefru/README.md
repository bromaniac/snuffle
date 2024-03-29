Downloaded from https://sources.vsta.org/comp.sources.unix/volume21/snefru/

See also: "A Fast Software One-Way Hash Function" by Ralph C. Merkle: https://link.springer.com/content/pdf/10.1007/BF00203968.pdf

Original usenet post:

> This is my revision of Ralph Merkle's SNEFRU program.  Snefru is a one-way
> hash algorithm:  given some input text, Snefru will come up with a single
> number such that no two texts will hash down to the same number.  In this
> way, Snefru can tell you whether an article has been corrupted, but not if
> it is authentic or not -- think of it as a super-strong checksum.
> 
> Starting with this posting, I am going to be using hashnews on all my
> c.s.u articles.  While I don't think that this is worth doing for most
> general Usenix articles, I think it will be an interesting experiment for
> archives.
> 
> I completely rewrote and reorganized the code that Ralph has made
> available.  For example, I split the comments out into manual pages, and
> put all the tests out into a separate program.  What I'm making available
> is a derived work, and therefore must be distributed under the same terms
> as Ralph's original code.  Thanks to him and Xerox for making his work
> available.  Some of the programs and manual pages are my original work,
> and therefore don't contain the Xerox copyright.  They are in the public
> domain, and feel free to do what you want with them.
> 
> This code needs a 32bit machine; good luck if you've only got 16 bits!
> 
> To compile, edit the Makefile if you use strchr/strrchr rather than
> index/rindex.  Also edit snefru.c to determine the byte order of your
> machine.  Once that's done, do "make tests" to verify the output.  If you
> get wrong answers, the first thing to suspect is the byte order.
> 
> Enjoy,
> Rich $alz <rsalz@bbn.com>
