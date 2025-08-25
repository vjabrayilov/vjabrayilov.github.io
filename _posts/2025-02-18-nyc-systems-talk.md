---
layout: distill
title: "Pushing Cloud Systems Toward Bare-Metal Performance"
description: "Reflections on my talk at NYC Systems about optimizing cloud infrastructure for maximum performance"
date: 2025-02-18
featured: true
tags: cloud-computing bare-metal performance systems nyc-systems
categories:
  - Talks
  - Systems

authors:
  - name: Vahab Jabrayilov
    url: "https://vjabrayilov.github.io"
    affiliations:
      name: CS, Columbia University
---

I had the incredible opportunity to speak at NYC Systems about pushing cloud systems toward bare-metal performance. It was a fantastic experience sharing ideas with the systems community and discussing the challenges and opportunities in bridging the performance gap between cloud and bare-metal infrastructure.

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">Had a great time speaking at NYC Systems today about pushing cloud systems toward bare-metal performance.<br>Big thanks to <a href="https://twitter.com/eatonphil?ref_src=twsrc%5Etfw">@eatonphil</a> for the invite, <a href="https://twitter.com/trailofbits?ref_src=twsrc%5Etfw">@trailofbits</a> for hosting, and the community for the engaging discussion! <a href="https://t.co/BRHgzxieXq">https://t.co/BRHgzxieXq</a></p>&mdash; Vahab Jabrayilov (@vjabrayilov7) <a href="https://twitter.com/vjabrayilov7/status/1958733254754017727?ref_src=twsrc%5Etfw">August 22, 2025</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

## The Performance Gap Challenge

The cloud has revolutionized how we deploy and scale applications, but it comes with inherent performance overhead. Traditional virtualization layers, network abstractions, and shared infrastructure all contribute to a performance gap when compared to bare-metal systems. This gap becomes particularly pronounced in performance-critical applications where every microsecond matters.

## Key Areas of Focus
During my talk, I talked about two of the systems that we have built at Columbia. 
### [Machnet](https://github.com/microsoft/machnet)
Despite a decade of research, most high-performance userspace network stacks remain impractical for public cloud tenants developing their applications atop Virtual Machines (VMs).

We identify two root causes: 
 - reliance on specialized NIC features (e.g., flow steering, deep buffers) absent in commodity cloud vNICs
 - rigid execution models ill-suited to diverse application needs. 
 
Machnet, a high-performance and flexible userspace network stack designed for public cloud VMs, uses only a minimal set of vNIC features that any major cloud provider supports. 
It also relies on a microkernel architecture to enable flexible application execution. 

I talked how we evaluated Machnet across three major public clouds and on production-grade applications, including a key-value store, an HTTP server, and a state-machine replication system.

Machnet is [open-source](https://github.com/microsoft/machnet)!

### Efficient Virtual Machine Scheduling

We have designed and built a highly efficient VM scheduler that operates at microsecond scale.

While I cannot share the technical details here at this stage, since the work is currently under submission to ASPLOS, I can say that it addresses long-standing challenges in virtualization performance. 

The goal is to enable tighter control over CPU resources in environments where latency and predictability are critical. I look forward to discussing the design and results once the review process is complete.

## The Future of Cloud Performance

The future of cloud computing lies not just in scalability and flexibility, but also in achieving performance levels that rival or even exceed traditional bare-metal deployments. This requires a holistic approach that considers hardware, software, and system design optimizations.

## Acknowledgments

Special thanks to [Phil Eaton](https://twitter.com/eatonphil) for the invitation and [Trail of Bits](https://twitter.com/trailofbits) for hosting this fantastic event. The NYC Systems community continues to be a vibrant forum for discussing cutting-edge systems research and engineering challenges.

The engaging discussion that followed the talk highlighted the importance of these performance optimizations in real-world deployments and the various approaches different organizations are taking to address these challenges.
