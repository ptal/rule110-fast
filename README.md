# Rule 110: Fast Version

For all source files, the code will be compiled with the following command to obtain the best performance:

```
g++ rule110.cpp -Wall -Werror -Wextra --pedantic -std=c++23 -march=native -DNDEBUG -O3 -o rule110
```

Make sure your code compiles with this command before submitting for review.

For debugging your code, you can compile with this command:
```
g++ rule110.cpp -Wall -Wextra --pedantic -std=c++23 -fopenmp -g -o rule110
```

You might need to add additional flags to use the C++ execution policy and OpenMP. You can give those commands below:

```
your compilation command
```

You can use `generator.cpp` to generate new automaton:

```
$ g++ -O3 -std=c++23 generator.cpp -o gen
$ ./gen --size 1M
$ ./rule110 --iter 1000 --init automaton_1M.txt
```

## Benchmarking Multithreaded Rule 110

## Profiling Multithreaded Rule 110

## Benchmarking and Profiling 1-byte-per-cell OpenMP Rule 110

## Benchmarking and Profiling Cache-friendly OpenMP Rule 110
