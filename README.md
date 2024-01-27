[![Actions Status](https://github.com/lizmat/App-Moarvm-Heapanalyzer/actions/workflows/test.yml/badge.svg)](https://github.com/lizmat/App-Moarvm-Heapanalyzer/actions)

NAME
====

App::MoarVM::HeapAnalyzer - MoarVM heap snapshot analysis tool

SYNOPSIS
========

    $ moar-ha file.snapshot

DESCRIPTION
===========

This is a command line application for analyzing MoarVM heap snapshots. First, obtain a heap snapshot file from something running on MoarVM. For example:

    $ raku --profile=heap something.raku

Then run this application on the heap snapshot file it produces (the filename will be at the end of the program output).

    $ moar-ha heap-snapshot-1473849090.9

Type `help` inside the shell to learn about the set of supported commands. You may also find [these](https://6guts.wordpress.com/2016/03/27/happy-heapster/) [two](https://6guts.wordpress.com/2016/04/15/heap-heap-hooray/) posts on the 6guts blog about using the heap analyzer to hunt leaks interesting also.

AUTHOR
======

Jonathan Worthington

COPYRIGHT AND LICENSE
=====================

Copyright 2016 - 2024 Jonathan Worthington

Copyright 2024 Elizabeth Mattijsen

This library is free software; you can redistribute it and/or modify it under the Artistic License 2.0.

