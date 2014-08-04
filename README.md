simhash
===========

This is a Python implementation of [Simhash](http://www.wwwconference.org/www2007/papers/paper215.pdf).

## Getting Started

<http://liangsun.org/posts/a-python-implementation-of-simhash-algorithm/>

## Build Status

[![Build Status](https://travis-ci.org/liangsun/simhash.png?branch=master)](https://travis-ci.org/liangsun/simhash)

## Differences in this fork

This fork of [liansung's simhash](https://github.com/liangsun/simhash) differs
in one important aspect: For the index of simhashes, the bucket keys and
offsets of a simhash are defined in the `Simhash` class instead of
`SimhashIndex`. This way, bucket keys can be calculated without having an
instance of `SimhashIndex` which is very convenient when persisting the bucket
keys in a database instead of in-memory.
