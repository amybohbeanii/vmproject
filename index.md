**Virtual Memory Implementation in C**

## Authors

Bonnie Ishiguro, Andrew Pan, Apurva Raman, Amy Wu 

## Quickstart

For setup and usage instructions see [README](https://github.com/amybohbeanii/vmproject/blob/master/README.md)

## Abstract
Our team project is to gain an understanding of virtual memory. An important part of virtual memory is the page fault handler, which becomes the focus of our learning. To achieve this goal, we built a fully functional demand paged virtual memory in C following the guidance of Notre Dame University’s VM project. This project implementation lets us understand the code mechanics of how the operating system handles page faults.

## Background
We focused our project on the implementation of a specific part of virtual memory, page replacement algorithms. This includes understanding how page faults occur and how to handle page faults by creating page replacement algorithms. A page fault occurs when the application uses the virtual memory, resulting in the page replace algorithm called by the user. There are many page replacement policies, such as random, first-in first-out (FIFO), least recently used (LRU), Second-chance, etc. The stretch goal was to include more advanced page replacement policies to make the process more optimal. Another stretch was to include a TLB table that makes paging more efficient. We decided to implement page replacement policies, random, fifo, and second-chance. We followed the architecture of implementing a frame table to understand how virtual memory is mapped to physical memory. 
The purpose of our project is to gain a general overview of Virtual Memory. We read ThinkOS Chapter 3: Virtual Memory to understand the different components that make up Virtual Memory (Refer to Figure 1). We read a previous project’s documentation on Virtual Memory in regard to Computer Architecture in order to understand that in the broader context, the concept of Virtual Memory is similar to caching. Understanding virtual memory is an important part of an Operating System and an implementation allows us to demonstrate mastery of the virtual memory concept. Specifically, our team was able to gain a comprehensive understanding of page faults, page table, frame table, disk, and page replacement algorithms random, fifo, and second-chance. 

## Implementation
Our goal for this project was to create a working virtual memory system to handle the mapping from virtual memory to physical memory. Due to the complexity of developing an entire virtual memory system with pages, frames, a page table, and the ability to write to disk, we chose to search for existing virtual memory projects and build upon those instead of creating a system entirely from scratch. We began with exploring virtual memory implementations on Arduino Uno’s and PintOS, a pseudo-OS developed for implementing different OS features as projects for a Stanford course.  After performing some preliminary implementation of both options, we chose to further explore the PintOS project with the intent of completing a virtual memory project in the OS.

After spending multiple weeks with trying to implement some of the features of PintOS necessary to begin working on virtual memory, we came to the conclusion that the multitude of issues we were running into from the OS was hindering our progress, and we pivoted our project to work on a different virtual memory project: Notre Dame’s Project V: Virtual Memory, which has a much simpler setup and a more readable code base.  The main goal of our new virtual memory project was to implement a page fault handler that would manage interactions with the page table and page replacement.

Our page fault handler is called whenever there is an attempted access to a page that is not mapped to a frame, or when there is an attempted write to a page when all of the pages in the table have an existing mapping.  We implemented multiple page replacement algorithms to address these issues, starting with a random page replacement as an MVP and eventually moving into FIFO page replacement with a circular buffer.


Results
Provide evidence demonstrating that what you built works. Though the details will be different for each project, screenshots and video are likely helpful. Include graphs or other data if appropriate.
 
In addition to creating your final report website, you will also perform two other tasks to prepare your work for release: clean up your code and write a README. Hopefully these should be trivial since you've been doing them all along.



## Results 

![Figure 1: Diagram of different components in VM](vm_diagram.jpg)

_Random_
_Fifo
_Second chance_

## Learning Objectives
This project was intended to be a learning exercise for the team to get hands on experience with implementing an important component of VM, the page fault handler. We accomplished the learning goals, which are:
- Learn about all the components of VM 
- In depth understanding of TLB
- In depth understanding of Page Table
- In depth understanding of different page replacement algorithms
- Mapping of Virtual Address to Physical Address
- Physical Memory versus Disk
- Design decisions on how to implement a frame table
Data structure decisions on how to implement fifo.

While there are various other page replacement algorithms to implement, this project still proves to be a valuable learning experience for the team to gain in-depth knowledge in VM and experience implementing some page replacement algorithms. 


