# DDFuzz

A prototype implementation of a novel instrumentation technique that adds data dependency information to traditional edge-coverage fuzzing.
The base code of the fuzzer relies on AFL++. To instrument a program with the data dependency pass, simply set the following environment variables before compiling:

`DDG_INSTR=1 AFL_LLVM_INSTRUMENT=classic make`

All the other aspects are the same as for vanilla AFL++. For more details, check out the paper *Fuzzing with Data Dependency Information*.
