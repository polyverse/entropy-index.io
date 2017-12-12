Entropy Index
==================

Summary
-------

The Entropy Index (EI) is measure of overall Entropy of a system; in terms of the difficulty of attacking or exploiting it.

EI is based on these three Axioms:
* EI is a number between 0 and 100.
* A system that is trivially hackable using an off-the-shelf exploit has an EI zero.
* A system that is impossible to compromise, using even the most adaptive exploit, has an EI of 100.

Measure of Efficacy; Not Technology
-------------------------------------

The fundamental definition of EI is bounded by efficacy *in face of attack*. We expect there to be many variables that capture diversity to be a part of EI, and for EI to be a very living definition that adapts to newer threat vectors as well as state-of-the-art defensive techniques.

Measuring Efficacy serves three purposes:
* EI is an effective number to help compare and contrast the defensive posture of two systems. 
  Especially for auditing and compliance.

* Help prioritizaton of cyber defense strategies to drive the most effective defense for the least investment.

* Prevent stagnation of working definition. As technologies and methodologies come and go, 
  the bounding conditions allow incorporating of new variables, and removal of irrelevant ones.

Motivation
----------

Static systems will always be compromised given enough time or resources. This is an intuitive axiomatic truth. If we consider the cost of attacking a static system to be O(1). There is a tradeoff between time and resources. You can parallelize over multiple attack vectors to cut down on time, or more conventionally, you can serially exploit one vector after another, and use fewer resources.

Therefore it stands to reason that an effective cyber defense strategy involves increasing the entropy of a system across multiple dimensions, most notably, time and space. 

* The more diversity there is across space (machines, clusters, datacenters, desktops, phones, laptops, tablets, etc.) the
  more difficult it becomes for an attacker to move laterally and establish persistence. They must have knowledge of that many
  different technologies and must carry a larger array of exploits, as opposed to repeating the exploit over and over again.
  
  However, given enough time a determined attacker could generate exploits at a cost of O(N), where N is the number of
  variants in play. Linear cost O(N) is definitely an improvement over constant cost O(1).
  
* The more diversity there is across time (use of different code, configuration, layouts, credentials, etc.) the higher the
  cost for an attacker to develop an exploit in terms of resources (thanks to the tradeoff mentioned above.) An effective
  attack must now be repeated at a cost of O(N) if there is diversity across space, M times where M is the number of diverse
  settings applied over a period of time. The cost of attack becomes at least geometric O(MN).

About
-----

The Entropy Index specification is authored and sponsored by [Polyverse Corporation](https://polyverse.io).

If you'd like to leave feedback, please [open an issue on
GitHub](https://github.com/polyverse/entropy-index.io/issues).


License
-------

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

Creative Commons - Attribution 4.0 International (CC BY 4.0)
https://creativecommons.org/licenses/by/4.0/
