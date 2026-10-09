# Basic Data Structures

Classroom implementations of B-tree insertion, Dijkstra shortest paths, Prim minimum spanning trees, and breadth-first traversal in Java, plus a Python directed-graph example. The sample output and source identifiers include Turkish course terminology.

## Java demo

The Java files declare package `com.tugcantopaloglu`. From the repository root with a JDK installed:

```sh
javac -encoding UTF-8 -d build Java/*.java
java -cp build com.tugcantopaloglu.Main
```

The demonstration uses embedded graph fixtures and prints each algorithm's results. It does not require a database or external library. Compile warnings about unchecked operations in `BFT.java` are present in the original exercise.

## Python graph example

Install the imported libraries in a separate environment and run the script:

```sh
python -m venv .venv
python -m pip install networkx matplotlib
python -X utf8 Python/main.py
```

Activate `.venv` before the install/run commands, or use that environment's Python executable explicitly. On Windows that is `.venv\\Scripts\\python.exe`; on Unix-like systems it is `.venv/bin/python`.

The Python script creates an in-memory directed graph, prints shortest paths, removes a vertex, and prints the remaining routes. `matplotlib` is imported even though the committed example does not display a plot. UTF-8 mode avoids encoding failures for Turkish output in redirected Windows terminals.

## Verification scope

The Java sources compiled and their sample `Main` executed with JDK 17. The Python example executed with Python 3.13, NetworkX, and Matplotlib. These demonstrations are educational examples, with no automated correctness suite for arbitrary graph inputs.
