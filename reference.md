# COURSE 1
## google test
https://google.github.io/googletest/quickstart-cmake.html

## CMAKE
https://cmake.org/cmake/help/latest/manual/cmake-generators.7.html

## Build process w/o IDE
```shell
cmake -S . -B build  # only need to execute one time, to create build dir
cmake --build build  # build every time after you modify or add new file
cd build && ./kuiper_datawhale_course1  # execute unit test
```

## Armdillo library
https://arma.sourceforge.net/docs.html#part_classes

## Code
需要注意的是，对矩阵进行指数运算不等于对矩阵中每个元素进行指数运算
例如，对矩阵A进行指数运算的结果为：

$$ e^A = \sum^{\inf}_{n=0}\frac{A^n}{n!} $$

这在armdillo中用expmat和exp进行区分