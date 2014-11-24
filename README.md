
# Pegleromyces

A runtime-mutable PEG parser for the
[Myco programming language](https://github.com/jemc/myco).

This is a design exercise to explore the weak points of the language,
while hopefully creating a viable candidate to replace the current parser
for the Myco interpreter with one that can be modified at runtime by user code.

Like [Pegarus](https://github.com/brixen/pegarus) for Ruby,
the implementation of Pegleromyces is based in part
on the parsing machine described in the paper:
["A Text Pattern-Matching Tool based on Parsing Expression Grammars"
by Roberto Ierusalimschy.](http://www.inf.puc-rio.br/~roberto/docs/peg.pdf)

## Design Goals

Pegleromyces is...

1. Implemented entirely in Myco.

2. Capable of interpreting grammars written in Myco.

3. Sophisticated enough to parse the Myco language itself.

4. Capable of allowing user-mutation of the grammar in between parse runs.

5. Capable of parsing composed grammars for other languages (including user-created languages).

6. Implemented as efficiently as possible given the above constraints.


## The Name

From [Wikipedia](https://en.wikipedia.org/wiki/Pegleromyces),

> Pegleromyces is a genus of fungi in the Tricholomataceae family.
> It is a monotypic genus, containing the single species
> Pegleromyces collybioides, found in Brazil and described as
> new to science by mycologist Rolf Singer in 1981.
