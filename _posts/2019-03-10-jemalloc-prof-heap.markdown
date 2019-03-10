---
layout: post
title:  "Jemalloc Prof Heap!"
date:   2019-03-10
tags:
    - C++ Linux
---

## Install Jemalloc

    -  bash autogen.sh
    -  ./configure --enable_prof
    -  make
    -  make install


## Export Linux Env
export MALLOC_CONF="prof:true",lg_prof_interval:30,lg_prof_sample:17

    which writes a profile to disk after every 1 GB of allocations, and records a stack trace every 128 kB.
    
    
## Run Program


## Gen pdf
./jemalloc/bin/jeprof --show_bytes --pdf /home/a.out /home/jeprof.15790.1.i1.heap > /tmp/call.pdf

<img src="{{ '/assets/img/touring.jpg' | prepend: site.baseurl }}" alt=""> 

