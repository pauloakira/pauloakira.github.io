---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

A PDF version is available [here](/files/cv.pdf) (drop a `cv.pdf` into the
`/files/` directory).

Education
======
* Ph.D. candidate, Escola Politécnica, Universidade de São Paulo (USP) — _expected YYYY_
* M.Sc. in _your program_, _your university_, _YYYY_
* B.Sc. in _your program_, _your university_, _YYYY_

Research interests
======
* Functional analysis and PDE analysis (Banach-space and variational methods)
* Virtual Element Method (VEM) — analysis and implementation
* Machine learning for PDEs — inductive bias, generalization, training objectives
* Approximation theory and error analysis of numerical schemes

Experience
======
* _YYYY – present_: **Data & AI Manager**, [Lyfe](#)
  * Lead the data & AI function

* _YYYY – present_: **PhD researcher**, Escola Politécnica, USP
  * Functional/PDE analysis applied to numerical methods (VEM) and ML for PDEs
  * Advisor: _name_

Skills
======
* **Programming**: Python, C/C++, MATLAB, Julia
* **Scientific computing**: FEM/VEM solvers, mesh generation, sparse linear algebra
* **Machine learning**: PyTorch, JAX, scikit-learn
* **Mathematics**: PDEs, functional analysis, probability, numerical analysis

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Service
======
* _Reviewer for ..._
* _Member of ..._
