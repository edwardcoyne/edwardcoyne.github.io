---
title: "Web Assembly (wasm)"
---

WebAssembly is an evolution of NaCl/pNaCL and asm.js. It is an effort to create a IR (intermediate format) for native code (C/C++ primarily) that is both portable and secure. It's primary intent is to allow native code to be distributed as part of a website and run in any browser; Mozilla, Microsoft, Apple, and Google are all signed on. While this part is cool, it isn't what I am interested in. 

I am interested in the fact that a lot of work has been put into developing a truely portable IR with solid SFI ([Software Fault Isolation](http://www.ece.cmu.edu/~ece732/readings/wahbe-sfi.pdf)) to allow safely sandboxed memory usage.

There is a LLVM frontend in active development for it that will compile C/C++ to wasm. Currently the wasm->machine code translation is happening in browser's javascript engines. 
