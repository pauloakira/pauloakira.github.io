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
`/files/` directory of the repo).

**Paulo Akira Figuti Enabe**
&nbsp;·&nbsp; <a href="mailto:paulo.enabe@usp.br">paulo.enabe@usp.br</a>
&nbsp;·&nbsp; +55 11 97205-0495
&nbsp;·&nbsp; Brazilian citizen

Education
======
* **Ph.D. in Structural Engineering**, Polytechnic School, University of São Paulo — _Sep. 2022 – Present_
* **M.Sc. in Structural Engineering**, Polytechnic School, University of São Paulo — _Apr. 2021 – Dec. 2021_
* **B.Sc. in Mechatronics Engineering**, Polytechnic School, University of São Paulo — _Mar. 2016 – Dec. 2020_

Complementary Education
======
* **Machine Learning Engineer Nanodegree**, Udacity — _May 2021 – Jul. 2021_
* **Exchange Program in Engineering**, Shibaura Institute of Technology, Tokyo, Japan — _Mar. 2019 – Jul. 2019_

Experience
======

**LyfeOS** — _Partner_, São Paulo &nbsp;·&nbsp; _Dec. 2023 – Present_
* Responsible for handling innovation in AI/ML.

**LyfeOS** — _Lead Data Engineer_, São Paulo &nbsp;·&nbsp; _Jul. 2023 – Present_
* Lead the Data Engineering team — defining data architecture, governance, and scalable infrastructure strategy.
* Head the AI/ML R&D team, overseeing research, experimentation, and production deployment of machine learning solutions.
* Architected and deployed a scalable cloud-based data lake, enabling centralized analytics and high-volume data processing.
* Designed and maintained end-to-end ML pipelines: data ingestion, feature engineering, model training, validation, and production monitoring.
* Built and orchestrated multi-agent AI systems to automate complex workflows, enabling autonomous task coordination and decision-making.
* Implemented MLOps / CI-CD practices for ML models, improving deployment reliability and time-to-production.

**Insper** — _Professor_, São Paulo &nbsp;·&nbsp; _Feb. 2023 – Present_
* Professor of Computational Mechanics.
* Research topics in Machine Learning and Numerical Methods.

**Accenture Global** — _Consultant_, São Paulo &nbsp;·&nbsp; _Sep. 2022 – Jul. 2023_
* AI and Data Lead in a Saudi Arabian bank.
* Software Engineer in a United Arab Emirates investment company.
* Software and Machine Learning Engineer in a UK telecommunications-company project.
* Tech Lead of a governance tool developed for Growth Studio.

**Accenture Brasil** — _Software Engineer_, São Paulo &nbsp;·&nbsp; _Dec. 2020 – Sep. 2022_
* Lead of a metaverse project, integrating business, creative, and technology.
* Lead of an applied-intelligence project, integrating business, creative, and technology.
* Led the AI team for research and development in the Labs department of Liquid Studios Brazil.
* Software engineer of a car-logistics project (designed an AWS-based solution).
* Software engineer in a telecommunications-company project.
* Head of an internal educational program teaching machine learning to non-specialist audiences.
* Developed cloud system architectures for ML and web applications.
* Developed system architectures for quadruped robots.
* Contributed to the quantum-computing group in the Labs department of Liquid Studios Brazil.

**Cambridge Family Enterprise Group** — _Summer Intern_, São Paulo &nbsp;·&nbsp; _Jan. 2019 – Feb. 2019_
* Worked on projects related to the governance of family-owned enterprises.
* Architected a database for prospecting family companies in Brazil.

**Offshore Mechanics Laboratory** — _Researcher_, São Paulo &nbsp;·&nbsp; _Dec. 2017 – Present_
* Research projects on marine structures, machine learning, and numerical methods.
* Started a research group focused on pure-mathematics topics.
* Co-advised undergraduate scientific-initiation students.

Projects
======

**Research in Applied Mathematics and Machine Learning** — _Dec. 2022 – Present_
* Developing a tensor manipulation library focused on deep learning.
* Designing compilers focused on numerical processes.
* Optimizing multi-head attention mechanisms in Transformer architectures.
* Developing Small Language Models with domain-specific knowledge.
* Research in numerical methods for Partial Differential Equations.

**Research in Applied Mathematics and Machine Learning** — _Dec. 2019 – present_
* Physics-Informed Neural Networks (PINNs) and their variants.
* Numerical methods with artificial neural networks, focused on approximation theory.
* Deep learning for nonlinear problems in solid mechanics.
* Applied functional analysis.
* Numerical methods for Partial Differential Equations.

**Applied Mathematics for Computer Simulation in Structural Engineering** — _Jul. 2019 – Dec. 2019_
* Virtual Element Method applied to rheological models.
* Alternative mathematical formulation for the Virtual Element Method.
* Graphical user interface (GUI) for the Virtual Element Method.
* Interface of pure and applied mathematics in complex systems.
* Numerical methods for Partial Differential Equations.

**Web application for Cursinho da Psico** _(social project for high-school students)_ — _Jul. 2019 – Dec. 2019_
* Built a web application supporting the social project's internal processes.

**Mathematics Coordinator — Cursinho da Psico** — _Dec. 2017 – Oct. 2019_
* Led the math faculty and taught classes in the social project Cursinho da Psico.

**Scientific Initiation in Engineering** — _Dec. 2017 – Oct. 2019_
* Research in structural engineering on the numerical simulation of wind turbines.

**Scientific Initiation in Mathematics** — _Jun. 2016 – Jan. 2018_
* Research in pure mathematics on real and functional analysis.

Languages
======
* **Portuguese** — native
* **English** — fluent
* **German** — basic
* **French** — basic

Skills
======
* **Programming languages**: Python, C/C++, C#, JavaScript
* **Tools / frameworks**: AWS, MATLAB, Figma, ROS/Gazebo, GitHub, Microsoft Office, Ansys, Abaqus, TensorFlow, PyTorch, MLflow, Optuna, Flask, Pandas, Angular, Node.js, Flutter, Next.js, React, LangChain

Publications
======
<ul>
{% assign pubs = site.publications | sort: 'date' | reverse %}
{% for post in pubs %}
  <li>
    <strong>{{ post.title }}</strong><br/>
    <span style="opacity:0.85">{{ post.authors }}</span><br/>
    <em>{{ post.venue }}</em>{% if post.arxiv %} &nbsp;·&nbsp; <a href="https://arxiv.org/abs/{{ post.arxiv }}">arXiv:{{ post.arxiv }}</a>{% endif %}{% if post.doi %} &nbsp;·&nbsp; <a href="https://doi.org/{{ post.doi }}">DOI</a>{% endif %}
  </li>
{% endfor %}
</ul>

Links
======
* [GitHub](https://github.com/pauloakira)
* [Lattes (CNPq)](http://lattes.cnpq.br/0653931190385652)
* [LinkedIn](https://linkedin.com/in/paulo-akira-enabe-732973172)
