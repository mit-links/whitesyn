# Whitesyn - A fully automatic test generation tool for performance bugs

## Purpose
This repository contains my Master Thesis from ETH Zurich (Computer Science).
The source code is not publicly available but might be requested from the [ETH Laboratory of Software Technology](https://www.lst.inf.ethz.ch/).

## Abstract
Unlike functional bugs, performance bugs are generally not well covered by unit tests in popular
software projects, even tough their presence may drastically decrease the performance of an
application. Usually, only a small group of developers maintain performance tests and they are
rarely updated. While tools for discovering potential performance issues exist, many require manual
work by a developer (e.g. writing tests or inspecting code), which may not be desirable.

This report presents an automatic test generation approach that uses static control-flow graph
analysis and a genetic algorithm. We have implemented this approach with the prototype tool
WhiteSyn, a fully automatic performance test generation tool. WhiteSyn is able to generate tests
with large input size, which is usually a prerequisite for performance bugs to manifest. With a static
analysis, WhiteSyn finds desired paths through a system under test and uses a genetic algorithm
to generate unit tests that trigger these paths and iterate desired loops multiple times. As a proof
of concept, WhiteSyn is able to generate tests that expose redundant computations, a common
class of performance bugs. Testing on known performance issues has shown that WhiteSyn is
able to generate tests with large input size and tests that expose previously known redundant
computations.
