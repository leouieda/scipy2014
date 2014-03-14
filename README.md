# Title

[Leonardo Uieda](http://www.leouieda.com),
[Vanderlei C. Oliviera Jr](http://fatiando.org/people/oliveira-jr),
[Valéria C. F. Barbosa](http://lattes.cnpq.br/0391036221142471)

## Brief Description

400 chars.

## Detailed Abstract

The inner properties of the Earth
can usually only be inferred
through indirect measurements of their effects.
For example,
density variations
cause disturbances in the gravity field
and seismic velocity variations
affect the path of seismic waves.
From a mathematical point of view,
this inference is an inverse problem.
To complicate things, geophysical inverse problems are usually ill-posed,
meaning that a solution:

* doesn't exist;
* exists but is non-unique;
* exists and is unique but is unstable;

These problems can usually be resolved
through least-squares estimation and regularization.

Research in geophysical inverse problems
involves the development of
new methodologies for parametrization,
different approaches to regularization,
new algorithms to handle large-scale problems,
combinations of existing methods,
etc.
All of the aforementioned
require the creation of software,
usually from scratch.
Furthermore,
most scientific software
are not designed with reuse in mind,
making remixing published methods difficult,
if not impossible.

We tackled these problems
by developing `fatiando.inversion`,
a framework for solving inverse problems
in [Fatiando a Terra](http://www.fatiando.org).
The goals of `fatiando.inversion` are:

* Enable writing code that
  intuitively maps to the theory (equations);
* Provide a consistent interface for all solvers
  (similar to that adopted by [scikit-learn](http://scikit-learn.org/));
* Automate the process of implementing a new inverse problem;
* Allow reuse and remixing with as little code as possible;

In this talk,
I'll briefly cover
the mathematics involved
and the design of our new API.
I'll walk through the process of
implementing a new inverse problem
(in about 30 lines of code)
using the example of
estimating the relief of a sedimentary basin
from its gravity anomaly.
Finally,
I'll conclude by outlining
how we are using this framework in our own research,
what we are currently working on,
and plans our for the future.










