## Implementation of Virtual Memory in C

## Authors

Bonnie Ishiguro

Andrew Pan

Apurva Raman

[Amy Wu](https://amybohbeanii.github.io/)

## Description

This student project was created as part of Olin College of Engineering’s Software Systems course. For more details on this project, see the final report.h

Virtual Memory is an important concept of an Operating System. To grasp the concept, our team decided to analyze the different components and techniques in VM. A comprehensive understanding of VM means knowing how virtual addresses are mapped to physical addresses. The concept is that virtual memory allows more memory to be used than physically available. The main component that allows this concept to work is the page table and the techniques are the various page replacement algorithms. 

## Setup and Usage

To compile the project from source, simply run `make` in the root directory.

To run the program: 
```
./virtmem npages nframes rand|fifo|custom scan|sort|focus
```
Examples to run the project:
```
./virtmem 15 10 rand sort
```
```
./virtmem 15 10 fifo focus
```
## Additional Libraries

## License 

MIT License
Copyright (c) [2017] [Bonnie Ishiguro, Andrew Pan, Apurva Raman, Amy Wu]

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

