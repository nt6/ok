# What

Here's a WIP implementation of the [K2 language](http://en.wikipedia.org/wiki/K_(programming_language)) in OCaml. Some basic things already work. A whole bunch of things does not yet.

# Why

fun, practice etc

# How

[Kona wiki](https://github.com/kevinlawler/kona/wiki) and [K2 reference](http://web.archive.org/web/20050504070651/http://www.kx.com/technical/documents/kreflite.pdf)

# Example

An example from [Ninety-Nine K problems](https://github.com/kevinlawler/kona/wiki/K-99%3A-Ninety-Nine-K-Problems):

~~~~
k) compress : {x@&1,~=':x}
k) compress["aaaaabbbccdddeee"]
(KCharArray (a b c d e))
k) ? "aaaaabbbccdddeee"  /same result using the range operator
(KCharArray (a b c d e))
~~~~

# Notes

Values are currently printed as S-expressions auto-generated by [core's](https://github.com/janestreet/core) Sexplib. Obviously, proper pretty-printing should be added eventually.

# Plan

Future priorities: correctness > completeness > code length / clarity > performance. So currently the code is

  - not too buggy
  - quite incomplete
  - way too long and a little weird
  - potentially very slow
