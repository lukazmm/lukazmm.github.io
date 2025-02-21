+++
title="Atmosphere: Towards Practical Verified Kernels in Rust"
date=2023-10-23

template="publication.html"

extra.journal="KISV '23: Proceedings of the 1st Workshop on Kernel Isolation, Safety and Verification"

[taxonomies]
# categories = ["Sample Post"]
# tags = ["post", "lorem"]
+++

This work applies a linearly typed extension of Rust and a newly developed SMT Verifier, Verus, to formally verify low-level operating system code.

**Citation**: *Atmosphere: Towards Practical Verified Kernels in Rust*. Xiangdong C., Zhaofeng L., Mesicek L., Narayanan V., and Burtsev A. Published in _KISV '23: Proceedings of the 1st Workshop on Kernel Isolation, Safety and Verification_.

**DOI**: [10.1145/3625275.3625401](https://doi.org/10.1145/3625275.3625401)

<!-- more -->

### Abstract

Historically, development of formally-verified operating systems was a challenging, time-consuming undertaking that relied on a narrow formal verification expertise and required many person-years of effort. We argue, however, that the balance of practicality is finally changing with development of automated verification tools that leverage a unique combination of the linear type system of Rust and automated verification based on satisfiability modulo theories (SMT). Our work leverages, Verus, a new SMT-based verifier for Rust, for development of a minimal yet practical microkernel, Atmosphere. Atmosphere is designed as a full-featured microkernel conceptually similar to the line of early L4 microkernels. We develop all code in Rust and prove its functional correctness, i.e., refinement of a high-level specification with Verus. Our experience shows that Verus provides a collection of practical features that significantly lower the burden of a verification effort making it possible to reason about correctness of the low-level systems code, e.g., low-level memory and address space management, recursive data structures like linked lists and page tables, etc. On average our code has proof-to-code ratio of 7.5:1 which is significantly lower than in prior approaches.

