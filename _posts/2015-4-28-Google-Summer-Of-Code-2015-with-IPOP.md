---
layout: post
title: Google Summer of Code 2015 with IPOP
---
<p align="center">
  <img src="/img/gsoc15.png" alt="GSoC 2015 Image"/>
</p>

I've been accepted for Google Summer of Code 2015 and I will be working on the IP-over-P2P (IPOP) Project. I thank Prof Renato, Mr. Kensworth and all the other members of the IPOP community for giving me this wonderful opportunity.<br><br>

IPOP is an open-source user-centric software virtual network allowing end users to define and create their own virtual private networks (VPNs). IPOP virtual networks provide end-to-end tunneling of IP or Ethernet over “TinCan” links setup and managed through a control API to create various software-defined VPN overlays.<br><br>
I will be working on the implementation of a controller framework, which will allow the users to plugin various independent modules, and create a controller according to the requirement. The new controller framework facililates easy extensibility of its functionality and eliminates the need for code changes to the framework when adding a new component.

### Project Abstract

The current implementation of IPOP controllers limits our ability to extend and configure controllers to exhibit different functionalities for different applications. The goal of this project is to create a flexible event-driven controller framework that provides a basis for next-generation IPOP controller designs. The framework should allow designers to “plug” independent modules that perform different core functions of an IPOP controller (e.g. IP address translation, topology management, routing, multicasting).

<br>
I will be mentored by Prof. Renato Figueiredo and Kensworth Subratie. Looking forward to an exciting summer working on this project :) 

