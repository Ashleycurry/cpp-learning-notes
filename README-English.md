# C++ Learning Notes

[中文](README.md) | [English](README-English.md)

A structured C++ learning notes repository covering C++ fundamentals, object-oriented programming, memory management, templates, and the Standard Template Library. The notes are intended for systematic study, review, and building a maintainable C++ knowledge base.

## Learning Path

```text
C++ Fundamentals
        ↓
Classes and Objects
        ↓
Memory Management
        ↓
Templates
        ↓
STL Overview
        ↓
string / vector / list / stack / queue
        ↓
Advanced Templates
```

Start with language fundamentals and basic classes, then move to object lifetime, resource management, and templates. After the STL chapters, practice the three levels of learning: use the interfaces, understand the underlying mechanisms, and extend or implement components.

## Course Index

| No. | Course material | Main topics |
| --- | --- | --- |
| 001 | [C++ Fundamentals](docs/001-C++入门基础.pdf) | C++ history, standard versions, course structure, and references |
| 002 | [Classes and Objects Part 1](docs/002-类和对象(上).pdf) | Class definitions, member functions, access control, encapsulation, and object basics |
| 003 | [Classes and Objects Part 2](docs/003-类和对象(中).pdf) | Default member functions, constructors, destructors, copy construction, and assignment |
| 004 | [Classes and Objects Part 3](docs/004-类和对象(下).pdf) | Initializer lists, implicit conversions, static members, friends, and nested classes |
| 005 | [Memory Management](docs/005-内存管理.pdf) | C/C++ memory layout, dynamic allocation, malloc/calloc/realloc/free, and new/delete |
| 006 | [Introductory Templates](docs/006-模板初阶.pdf) | Generic programming, function templates, class templates, and template parameters |
| 007 | [STL Overview](docs/007-STL简介.pdf) | STL components, its six major parts, learning methods, and practical value |
| 008 | [string](docs/008-string.pdf) | `std::string`, common APIs, iterators, range-based for, and `auto` |
| 009 | [vector](docs/009-vector.pdf) | Construction, iterators, capacity, storage management, insertion, deletion, and access |
| 010 | [list](docs/010-list.pdf) | Linked-list containers, iterators, capacity, element access, insertion, and deletion |
| 011 | [stack and queue](docs/011-stack和queue.pdf) | Stack, queue, adapters, minimum stack, expression evaluation, and sequence problems |
| 012 | [Advanced Templates](docs/012-模板进阶.pdf) | Non-type template parameters, specialization, partial specialization, and matching |

## Core Topics

### C++ Fundamentals

- Understand how C++ evolved from C and how the language standards developed.
- Distinguish the language, the standard library, and the STL.
- Build the habit of consulting standard and library documentation.

### Classes and Objects

- Define data and behavior with `class`.
- Understand encapsulation, access control, and member functions.
- Learn constructors, destructors, copy constructors, and assignment operators.
- Understand compiler-generated default member functions and when to implement them manually.
- Use initializer lists correctly for references, `const` members, and members without default constructors.

### Memory Management

- Distinguish stack, heap, static storage, constant storage, and code regions.
- Understand dynamic allocation, release, and growth.
- Distinguish C-style `malloc/free` from C++-style `new/delete`.
- Watch for leaks, dangling pointers, double frees, and out-of-bounds access.

### Templates and Generic Programming

- Use function and class templates to write type-independent code.
- Understand template instantiation and argument deduction.
- Study non-type template parameters, specialization, and partial specialization.
- Balance reuse, readability, and compile-time complexity.

### STL and Containers

- Understand the relationship between containers, iterators, algorithms, and function objects.
- Use `string` for managed string storage and common operations.
- Understand contiguous `vector` storage, `size`, `capacity`, `resize`, and `reserve`.
- Understand `list` nodes, iterators, and insertion/deletion trade-offs.
- Use `stack` and `queue` for last-in-first-out and first-in-first-out problems.

## Study Recommendations

1. Read each course material once to build a concept map.
2. For every interface, record its purpose, complexity, preconditions, and invalidation rules.
3. Do not only memorize STL APIs; study the underlying data structures.
4. Turn code fragments from the materials into independent experiments.
5. For resource-management code, inspect object lifetime and failure paths carefully.
6. When studying templates, pay attention to deduction, instantiation, and compiler diagnostics.
7. Use standard documentation to verify details instead of treating one compiler's behavior as the language standard.

## General Build Commands

The repository currently focuses on course materials. If standalone `.cpp` examples are added later, use a compiler that supports C++11 or newer:

```bash
g++ -std=c++11 -Wall -Wextra -Wpedantic example.cpp -o example
```

For newer language features:

```bash
g++ -std=c++17 -Wall -Wextra -Wpedantic example.cpp -o example
```

On Windows, MinGW-w64, Visual Studio, or another toolchain with modern C++ support can be used.

## Current Scope

- The repository contains numbered C++ PDF course materials.
- The materials cover language fundamentals, object-oriented programming, memory management, templates, and STL.
- There is currently no standalone `src` examples directory.
- There is currently no unified build system, test suite, or executable application.

## Possible Extensions

- Add independent `.cpp` examples for each chapter.
- Add a CMake build configuration.
- Add unit tests and container experiments.
- Add notes on complexity, iterator invalidation, and exception safety.
- Add modern C++ topics such as smart pointers, move semantics, lambdas, concurrency, and ranges.

## References

- [C++ Fundamentals](docs/001-C++入门基础.pdf)
- [Classes and Objects Part 1](docs/002-类和对象(上).pdf)
- [Classes and Objects Part 2](docs/003-类和对象(中).pdf)
- [Classes and Objects Part 3](docs/004-类和对象(下).pdf)
- [Memory Management](docs/005-内存管理.pdf)
- [Introductory Templates](docs/006-模板初阶.pdf)
- [STL Overview](docs/007-STL简介.pdf)
- [string](docs/008-string.pdf)
- [vector](docs/009-vector.pdf)
- [list](docs/010-list.pdf)
- [stack and queue](docs/011-stack和queue.pdf)
- [Advanced Templates](docs/012-模板进阶.pdf)
