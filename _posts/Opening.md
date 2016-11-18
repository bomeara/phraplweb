---
layout: post
title: What is PHRAPL?
---

For phylogenetics we routinely search over large tree spaces, but typically assume that there is no gene flow between species. In population genetics, we often assume population shared history does not matter, but gene flow between populations is of great importance. Phylogeography spans both of these areas. Typically, this is dealt with by ignoring gene flow, ignoring structure, or by trying just a few examples of possible branching and gene flow scenarios. PHRAPL can create hundreds of possible histories that have a mixture of gene flow, population subdivision, and/or population size differences and compare these models using AIC. Not all these models have analytic solutions, so we simulate to estimate the likelihoods. This is similar to approximate Bayesian computation, but is prior-free (which could be good or bad, depending on your perspective) and uses the gene tree topology as a summary stat.