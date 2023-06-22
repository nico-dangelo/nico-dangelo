---
title: Network Robustness, part 1
author: Nico D'Angelo
date: '2023-06-21'
slug: network-robustness-part-1
categories: ["Networks"]
tags: ["Robustness"]
draft: TRUE
---

## Preliminaries

For anyone reading this who is not a network scientist, we need to cover some basic concepts and definitions before we can dive into the properties that make a network robust. [Almost every journal article in Network Science starts with this anyway]

### Networks and their representations

A **network** is an abstraction for a set of objects, for which the set of connections between them is important. This can be a group of people (usually called a "social network,") a power grid, an ecosystem of animal or plant species, a public transportation system, etc.Network Science uses tools from a subdiscipline of mathematics called Graph Theory to represent, describe, and analyze networks and processes that occur on them. 

A graph `\(G\)` is a mathematical object, given by a pair of sets: `\(G=(V,E)\)`. Here, `\(V\)` is the set of **vertices** (also called "nodes," "actors," or "agents") representing the objects in the system we're interested in, and `\(E\)` is the set of **edges** (also called "ties," among other things) representing some kind of connection between the nodes in `\(V\)`. By convention, I'll use "nodes" and "edges." It's also useful to have symbols defined for the cardinalities (sizes) of these sets, as they'll come up often in calculations.
