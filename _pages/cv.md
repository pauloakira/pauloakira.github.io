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
* Ph.D. in _your program_, _your university_, _expected YYYY_
* M.Sc. in _your program_, _your university_, _YYYY_
* B.Sc. in _your program_, _your university_, _YYYY_

Research interests
======
* Virtual Element Method (VEM) and Finite Element Method (FEM)
* Scientific machine learning and physics-informed models
* Probability theory and stochastic analysis for numerical methods
* Functional analysis and approximation theory

Experience
======
* _YYYY – present_: PhD researcher, _your group / lab_
  * _Brief description of your work_
  * Advisor: _name_

* _YYYY – YYYY_: _Position_, _Institution_
  * _Brief description_

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
