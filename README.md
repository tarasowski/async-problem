# JavaScript has a problem

We like to say that JavaScript has a callback problem<sup>†</sup>.
This project considers various approaches to the following problem:

*Given a path to a directory containing an index file, __index.txt__, and
zero or more other files, read the index file (which contains one filename
per line), then read each of the files listed in the index concurrently,
concat the resulting strings (in the order specified by the index), and
write the result to stdout.*

*The program's exit code should be 0 if the entire operation is successful;
1 otherwise.*

All side effects must be isolated to the `main` function. Impure functions
may be defined at the top level but may only be invoked in `main`.

The solutions are best read in the following order:

  - [__synchronous.js__](./synchronous.js)
  - [__callbacks.js__](./callbacks.js)
  - [__node-streams.js__](./node-streams.js)
  - [__async.js__](./async.js)
  - [__righto.js__](./righto.js)
  - [__promises.js__](./promises.js)
  - [__promises-pipe.js__](./promises-pipe.js)
  - [__bluebird-promisell.js__](./bluebird-promisell.js)
  - [__most.js__](./most.js)
  - [__coroutines-co.js__](./coroutines-co.js)
  - [__coroutines-bluebird.js__](./coroutines-bluebird.js)
  - [__promise-chaining.js___](./promise-chaining.js)
  - [__await.js__](./await.js)
  - [__futures.js__](./futures.js)
  - [__callbacks-revenge.js__](./callbacks-revenge.js)

The above ordering is suggested reading order only – not grade. Solutions are
graded on the following criteria:

  - the size of `main` (smaller is better); and
  - the degree to which the approach facilitates breaking the problem into
    manageable subproblems.

---

† Perhaps in five years we'll be saying that JavaScript has a promise problem.
