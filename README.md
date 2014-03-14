# Title

[Leonardo Uieda](http://www.leouieda.com),
[Vanderlei C. Oliviera Jr](http://fatiando.org/people/oliveira-jr),
[Valéria C. F. Barbosa](http://lattes.cnpq.br/0391036221142471)

## Brief Description

400 chars.

## Detailed Abstract

The inner properties of the Earth can usually only be inferred through indirect measurements of their effects.

For example, density variations cause disturbances in the gravity field
and seismic velocity variations affect the path of seismic waves.

From a mathematical point of view, this inference is an inverse problem.

To complicate things, geophysical inverse problems are usually ill-posed.

This means that the solution to the problem:

* doesn't exist;
* exists but is non-unique;
* exists and is unique but is unstable;

These problems can be resolved through least-squares estimation and regularization.

Regularization is the mathematical process through which we insert into the inverse problem our prior physical and geological knowledge.

Research in geophysical inverse problems involves the development of new methodologies
for parametrization, different approaches to regularization, new algorithms to
handle large-scale problems, combinations of existing methods, etc.

Research involves the development of software to test and analyse these new methods.

Source code for the software developed for publications is rarely available.

Software is usually recreated from scratch or by copy-and-pasting existing code.

Software is not designed with reuse in mind.

This leads to a constant "reinvention of the wheel" and makes remixing published methods difficult, if not impossible.


We tackled these problems by developing `fatiando.inversion`, a framework for solving inverse problems in [Fatiando a Terra](http://www.fatiando.org).

Fatiando already offers a range of forward modeling modules that can be used in conjunction.

The goals of `fatiando.inversion` are:

* Enable writing code that intuitively maps to the theory (equations);
* Provide a consistent interface for all solvers (similar to that adopted by [scikit-learn](http://scikit-learn.org/));
* Automate as much as possible the process of implementing a new inverse problem;
* Allow reuse and remixing with as little code as possible;

In this talk, I'll first very briefly cover the mathematics involved,
then I'll show how we mapped that to the source code to design our API.

Throughout the talk, I'll refer to the example of estimating the relief of a sedimentary basin from its gravity anomaly.

This example will serve to walk through the process of implementing a new inverse problem in approximately 30 lines of code using `fatiando.inversion` and the existing forward modeling functions.

Finally, I'll conclude by outlining how we are using this framework for our research in the [PINGA lab](https://github.com/pinga-lab),
current efforts to expand this framework, and our plans for the future.










