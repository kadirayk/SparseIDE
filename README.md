# SparseIDE

This repository contains the SparseIDE framework proposed in our ICSE 2024 paper: "Symbol-Specific Sparsification of Interprocedural Distributive Environment Problems".  

## Content

1. SparseIDE implementation source code: `SparseHeros`  
2. Constant Propagation Analysis Client source code: `SparseIDEClient`
3. ConstantBench microbenchmark test cases: `SparseIDEClient/src/test/java/target/constantbench`

## Building the Client from the Source

1. Install the dependencies for `SparseIDEClient`: run `bash install_dependencies.sh` under `SparseIDEClient/dependencies`
2. Build the executable: run `mvn clean install` (Note that *install* will also run the correctness test cases on the ConstantBench)
3. Find the executable jar, `SparseIDEClient-0.0.1-SNAPSHOT-jar-with-dependencies.jar` under `SparseIDEClient/target`

## Using the SparseIDE Framework

SparseIDE extends the popular [Heros IFDS/IDE Solver](https://github.com/soot-oss/heros)

To build and use SparseIDE:

1. run `mvn clean install` in `SparseHeros`
2. add the following dependency to your project:

```xml
<dependency>
    <groupId>de.upb.cs.swt</groupId>
    <artifactId>heros</artifactId>
    <version>1.2.3-Sparse-SNAPSHOT</version>
</dependency>
```
