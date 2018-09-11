---
title: "Artificial Intelligence, Data Science and Machine Learning Systems Design"
abstract: >
  Machine learning solutions, in particular those based on deep learning methods, form an underpinning of the 
  current revolution in “artificial intelligence” that has dominated popular press headlines and is having a 
  significant influence on the wider tech agenda.
  
  In this talk I will give an overview of where we are now with machine learning solutions, and what challenges 
  we face both in the near and far future. These include practical application of existing algorithms in the 
  face of the need to explain decision making, mechanisms for improving the quality and availability of data, 
  dealing with large unstructured datasets.
ipynb: 2018-11-30-artificial-intelligence-data-science-and-machine-learning-systems-design.ipynb
reveal: 2018-11-30-artificial-intelligence-data-science-and-machine-learning-systems-design.slides.html
author:
- family: Lawrence
  given: Neil D.
  gscholar: r3SJcvoAAAAJ
  institute: Amazon Cambridge and University of Sheffield
  twitter: lawrennd
  url: http://inverseprobability.com
date: 2018-11-30
venue: Fifth International Workshop on Sustainable Road Freight, Cambridge
transition: None
---

\include{talk-macros.tex}

\include{_data-science/includes/gartner-hype-cycle-bd-ds-iot-ml.md}
\include{_data-science/includes/lies-damned-lies.md}
\include{_ml/includes/what-is-ml.md}
\include{_ml/includes/data-science-vs-ai.md}
\include{_ai/includes/embodiment-factors.md}
\include{_data-science/includes/evolved-relationship.md}
\include{_ml/includes/what-does-machine-learning-do.md}

\newslide{Deep Learning}

* These are interpretable models: vital for disease etc.

* Modern machine learning methods are less interpretable

* Example: face recognition

\include{_ml/includes/deep-learning-overview.md}
\include{_gp/includes/gp-intro-very-short.md}
\include{_deepgp/includes/deep-olympic.md}

\include{_data-science/includes/a-time-for-professionalisation.md}
\include{_data-science/includes/the-data-crisis.md} 

\newslide{Rest of this Talk: Two Areas of Focus}

* Reusability of Data

* Deployment of Machine Learning Systems

\newslide{Rest of this Talk: Two Areas of Focus}

* <s>Reusability of Data</s>

* Deployment of Machine Learning Systems

\include{_data-science/includes/data-readiness-levels.md}

\newslide{Artificial Intelligence}

* Challenges in deploying AI.

* Currently this is in the form of "machine learning systems"

\newslide{Internet of People}

* Fog computing: barrier between cloud and device blurring.
    * Computing on the Edge

* Complex feedback between algorithm and implementation
  
\newslide{Deploying ML in Real World: Machine Learning Systems Design}

* Major new challenge for systems designers.

* Internet of Intelligence but currently:
	* AI systems are *fragile*

\include{_ai/includes/ml-systems-design-long.md}
\include{_uq/includes/uncertainty-quantification.md}

\newslide{Conclusion}

* Artificial Intelligence and Data Science are fundamentally different.

* In one you are dealing with data collected by happenstance.

* In the other you are trying to build systems in the real world, often by actively collecting data.

* Our approaches to systems design are building powerful machines that
will be deployed in evolving environments.

\newslide{Thanks!}

\slides{
* twitter: \@lawrennd
* blog: [http://inverseprobability.com](http://inverseprobability.com/blog.html)
* [Natural vs Artifical Intelligence](http://inverseprobability.com/2018/02/06/natural-and-artificial-intelligence)
* [Mike Jordan's Medium Post](https://medium.com/@mijordan3/artificial-intelligence-the-revolution-hasnt-happened-yet-5e1d5812e1e7)
}