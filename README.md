# Simple arxiv scrapper

Use the python package [here](https://github.com/lukasschwab/arxiv.py) for easy scrapping:

## Usage 

### Let's search for "quantum mechanics"

```
arxiv quantum AND mechanics  # see arxiv API for keywords similar to AND

0) "Einstein's Dream" - Quantum Mechanics as Theory of Classical Random Fields
1) On a New Form of Quantum Mechanics (II)
2) On Finite $J$-Hermitian Quantum Mechanics
3) Probabilistic foundations of quantum mechanics and quantum information
4) Bhomian Mechanics vs. Standard Quantum Mechanics: a Difference in Experimental Predictions
5) About quantum mechanics interpretation
6) The Postulates of Quantum Mechanics
7) Quantum Statistical Mechanics. III. Equilibrium Probability
8) Naïve Physics and Quantum Mechanics: The Cognitive Bias of Everett's Many-Worlds Interpretation
9) Causality and probabilistic interpretation of quantum mechanics


# (for abstract)|M(ore results)/F(lip sorting)/Q(uit)
```

The output by default is sorted by relevance. Here on 

- `M/m` will give 10 more results
- `F` will flip to top 10 chronological papers satisfying search query
- `#` will give abstract, with author name, journal name, date - see next example

## Downloading

In above list, if I select 6, I get

```
Title: The Postulates of Quantum Mechanics


Journal: None
Category: physics.ed-ph
Last updated: 2006-02-21 16:52:37+00:00
Orig. published: 2006-02-21 16:52:37+00:00
V. Dorobantu


As a starting point in understanding Quantum Mechanics, the postulates of
Quantum Mechanics are presented, and few of the main eigenvalue problems, as
well.


Download Y/n?

```

Pressing `Y/y` will download the file to current directory (by default). 


## Todo

1. Make the downloading asynchronous
2. Add easy way to customize the download directory
