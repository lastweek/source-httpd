# Httpd

The code is well-structured. I believe once we acquire the coding conventions,
it should be easier to read the code.

Projects like this must have a lot internal neat facilities.
For instance, logging, buffer mgmt, http response generation (a lot string parsing).


Several things I was interested but didn't have time to cover
1. How it handles a new http request? More specific, threading model, buffer mgmt (mmap?),
and external module invocation (e.g., how it runs server Java, Node.Js code)?
2. The mmap/munmap usages. httpd server was used by many TLB-opt papers just
because it has a not-so-good usages of mmap/munmap (coz munmap brings TLB shootdowns).
3. Security hadening. How this is carried out?
