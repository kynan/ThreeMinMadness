class: center, middle, inverse

# Productive and Efficient Computational Science Through Domain-specific Abstractions

## **Florian Rathgeber**<sup>1</sup>
## Supervisors: David Ham<sup>1,2</sup>, Paul Kelly<sup>1</sup>

.footnote[<sup>1</sup> Department of Computing, Imperial College London
<sup>2</sup> Department of Mathematics, Imperial College London]

---

## Scientific Software

### Ideal world
* computationally efficient
* maintainable
* composable
* allow scientists to work very productively

--

### Reality
* solve a very specific research problem
* for a specific kind of user
* on a particular hardware platform

--

### Solution?

Get the abstractions right!

---

.scale[![Firedrake](http://firedrakeproject.org/_static/banner.png)]

> Firedrake is an automated system for the portable solution of partial
> differential equations using the finite element method (FEM).
>
> .source[&mdash; firedrakeproject.org]

--

Two-layer abstraction for finite element computation from high-level descriptions:
* Firedrake: a portable finite element computation framework  
  *Drive FE computations from a high-level problem specification*
* PyOP2: a high-level interface to unstructured mesh based methods  
  *Efficiently execute kernels over an unstructured grid in parallel*

---

background-image:url(images/fem.svg)

---

## The Firedrake/PyOP2 tool chain

![Firedrake](images/firedrake_toolchain.svg)

---

## Two-layered abstraction: Separation of concerns

![Separation of concerns](images/firedrake_toolchain_users.svg)
