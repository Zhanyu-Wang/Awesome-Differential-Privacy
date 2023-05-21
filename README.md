# Awesome-Differential-Privacy-for-Statisticians

## What is special about 'DP for STAT'?
1. Knowledge about the population instead of the sample. 
2. Quantification of uncertainty from various sources (sampling error + noise for privacy protection). 
3. Art of the tradeoff between statistical utility and privacy. 

---
(This part is for general readers including statisticians.)
## Intro for beginners
- [Why differential privacy is awesome](https://desfontain.es/privacy/differential-privacy-awesomeness.html)
- [Differential Privacy: An Introduction for First Graders](https://www.dataversity.net/differential-privacy-an-introduction-for-first-graders/#)
- [Differential privacy, an easy case](https://accuracyandprivacy.substack.com/)
- [Differential Privacy: A Primer for a Non-technical Audience (2017)](https://privacytools.seas.harvard.edu/files/privacytools/files/pedagogical-document-dp_0.pdf)
- [Challenges towards the Next Frontier in Privacy (2023)](https://arxiv.org/pdf/2304.06929.pdf)

## What are the privacy issues when not using DP?
- [Potential privacy lapse found in Americans’ 2010 census data - AP News](https://apnews.com/article/aba8e57c145047b5bab11b62baaa7f7a)
- [Poking Holes in Genetic Privacy - The New York Times](https://www.nytimes.com/2013/06/18/science/poking-holes-in-the-privacy-of-dna.html)
- [NetFlix Cancels Recommendation Contest After Privacy Lawsuit](https://www.wired.com/2010/03/netflix-cancels-contest/)
- [Your Data Were ‘Anonymized’? These Scientists Can Still Identify You](https://www.nytimes.com/2019/07/23/health/data-privacy-protection.html)

Maybe it is necessary to emphasize: [Statistical Inference is Not a Privacy Violation](https://differentialprivacy.org/inference-is-not-a-privacy-violation/)

What about other privacy protection techniques, e.g., tokenization, masking, k-anonymity? They will fail in some cases. See this blog: [What anonymization techniques can you trust?](https://desfontain.es/privacy/trustworthy-anonymization.html)

## Who are using DP?
The list below is from this report: [Technology Factsheet: Differential Privacy.](https://www.belfercenter.org/sites/default/files/files/publication/diffprivacy-3.pdf)  Authors: Raina Gandhi, Amritha Jayanti. Related: Alexandra Wood, Michael B. Hawes. Fall 2020.
- [US Census (2020)](https://www.nytimes.com/2018/12/05/upshot/to-reduce-privacy-risks-the-census-plans-to-report-less-accurate-data.html): with [ε=19.61](https://www.census.gov/newsroom/press-releases/2021/2020-census-key-parameters.html)
- [Google Chrome](https://static.googleusercontent.com/media/research.google.com/de//pubs/archive/42852.pdf): [(RAPPOR with ε=2 for particular data, and ε=8 or 9 over the lifetime of the user)](https://www.wired.com/story/apple-differential-privacy-shortcomings/)
- [Apple](https://docs-assets.developer.apple.com/ml-research/papers/learning-with-privacy-at-scale.pdf): [(official budget explanation)](https://www.apple.com/privacy/docs/Differential_Privacy_Overview.pdf) [(MacOS10.12 with ε=6, iOS10 with ε=14, iOS11 Beta with ε=43)](https://www.wired.com/story/apple-differential-privacy-shortcomings/)
- [Uber](https://www.wired.com/story/uber-privacy-elastic-sensitivity/): [Differential Privacy at Scale: Uber and Berkeley Collaboration](https://www.usenix.org/conference/enigma2018/presentation/ensign)
- [Microsoft](https://blogs.microsoft.com/ai-for-business/differential-privacy/), [Facebook](https://research.facebook.com/blog/2020/06/protecting-privacy-in-facebook-mobility-data-during-the-covid-19-response/), [Amazon](https://github.com/awslabs/sagemaker-privacy-for-nlp), [Snapchat](https://eng.snap.com/device-distributed-machine-learning), [LinkedIn](https://arxiv.org/pdf/2002.05839.pdf)
- ...

The table below is from this paper in 2020: [LinkedIn’s Audience Engagements API: A Privacy Preserving Data Analytics System at Scale](https://arxiv.org/pdf/2002.05839.pdf)

| Use Case |  Privacy    Model  |  DP Algorithm    Parameters  $(\epsilon, \delta)$ |  Daily DP    Parameters  $\left(\epsilon_{day}, \delta_{day} \right)$ |  Monthly DP    Parameters  $\left(\epsilon_{month} , \delta_{month} \right)$ |
| :---: | :---: | :---: | :---: | :---: |
|  Google - RAPPOR     Chrome Homepages  | Local | (0.534,0) | (25.63,0) 30 min reporting  | (769,0) |
|  Apple - Safari    Domains   | Local | (4,0) | (8,0) | (240,0) |
| Apple - Emojis  | Local |(4,0) | (4,0) | (120,0) |
|  Microsoft - Telemetry    Collection per App  | Local  | (0.686,0) | (2.74,0)   hour reporting  | (82.2,0) |
|  Google - Mobility    Reports   | Global | (0.11,0)  or  (0.22,0) | (2.64,0) | (79.2,0) |
|  Microsoft - Assistive    AI  | Global | $(4,10^{-7})$ | Not available | Not available |
|  LinkedIn - Audience    Engagement API  | Global | $(0.15,10^{-10})$ | - | $(34.9,7 \times 10^{-9})$ |

---

## Statisticians' slides
- Vishesh Karwa. [Differential Privacy and Statistical Inference: A statistician’s perspective.](https://simons.berkeley.edu/sites/default/files/docs/6713/karwa-statisticalinferenceandprivacy.pdf) 2017.
- Aleksandra Slavković. [Differentially Private Estimators & Basic Statistical Inference.](http://helper.ipam.ucla.edu/publications/data2010/data2010_8553.pdf) 2010.
- John C. Duchi. [Local Privacy, Statistical Minimax Rates, and Learning.](https://web.stanford.edu/~jduchi/projects/DuchiJoWa13_talk.pdf) 2013.

## Papers
Note that this is not a full list, but I will try to make it as comprehensive as possible.
### Top Statistics journals
#### JASA
- Wasserman, Larry, and Shuheng Zhou. "A statistical framework for differential privacy." 2010.
- Duchi, John C., Michael I. Jordan, and Martin J. Wainwright. "Minimax optimal procedures for locally private estimation." 2018. (Discussion.)
- Awan, Jordan, and Aleksandra Slavković. "Structure and sensitivity in differential privacy: Comparing k-norm mechanisms." 2021.
- Avella-Medina, Marco. "Privacy-preserving parametric inference: a case for robust statistics." 2021.
- Drechsler, Jörg. "Differential Privacy for Government Agencies—Are We There Yet?." 2023.

#### Annals of Statistics
- Karwa, Vishesh, and Aleksandra Slavković. "Inference using noisy degrees: Differentially private β-model and synthetic graphs." 2016.
- Tian, Xiaoying, and Jonathan Taylor. "Selective inference with a randomized response." 2018.
- Rohde, Angelika, and Lukas Steinberger. "Geometrizing rates of convergence under local differential privacy constraints." 2020.
- Cai, T. Tony, Yichen Wang, and Linjun Zhang. "The cost of privacy: Optimal rates of convergence for parameter estimation with differential privacy." 2021.

#### Journal of the Royal Statistical Society. Series B (Statistical Methodology)
- Dong, Jinshuo, Aaron Roth, and Weijie J. Su. "Gaussian differential privacy." 2022.

#### Journal of the Royal Statistical Society. Series A (Statistics in Society)
- Lei, Jing, Anne-Sophie Charest, Aleksandra Slavkovic, Adam Smith, and Stephen Fienberg. "Differentially private model selection with penalized and constrained likelihood." 2018.

#### Bernoulli
- Butucea, Cristina, et al. "Local differential privacy: Elbow effect in optimal density estimation and adaptation over Besov ellipsoids." 2020.
- Lam-Weil, J., Laurent, B., & Loubes, J. M. ["Minimax optimal goodness-of-fit testing for densities and multinomials under a local differential privacy constraint."](https://arxiv.org/pdf/2002.04254.pdf) 2022.

#### Annual Review of Statistics and Its Application
- Reiter, Jerome P. "Differential privacy and federal data releases." 2019.
- Slavković, Aleksandra, and Jeremy Seeman. "Statistical data privacy: A song of privacy and utility." 2023.
- Craiu, Radu V., Ruobin Gong, and Xiao-Li Meng. "Six Statistical Senses." 2023.
- Abowd, John M., and Michael B. Hawes. ["Confidentiality protection in the 2020 US Census of population and housing."](https://www.annualreviews.org/doi/full/10.1146/annurev-statistics-010422-034226) 2023.

#### Statistical Science
- Bowen, Claire McKay, and Fang Liu. "Comparative study of differentially private data synthesis methods." 2020.

### Other journals
- Dwork, Cynthia, and Adam Smith. ["Differential privacy for statistics: What we know and what we want to learn."](https://journalprivacyconfidentiality.org/index.php/jpc/article/download/570/553/584) Journal of Privacy and Confidentiality 1.2 (2010).
- Duchi, John C., Michael I. Jordan, and Martin J. Wainwright. ["Local privacy and statistical minimax rates."](https://ieeexplore.ieee.org/abstract/document/6686179/) 2013 IEEE 54th Annual Symposium on Foundations of Computer Science. IEEE, 2013.

### Thesis 
- Zhang, Huanyu. ["Statistical inference in the differential privacy model."](https://ecommons.cornell.edu/handle/1813/110688) (2021).  Diss. Cornell University.
- Wang, Yichen. ["Topics In Differentially Private Statistical Inference"](https://repository.upenn.edu/edissertations/5529/) (2022). Publicly Accessible Penn Dissertations. 5529.

---

## Professional blogs
- [DifferentialPrivacy.org](https://differentialprivacy.org/)
- [Ted is writing things: On privacy, research, and privacy research.](https://desfontain.es/privacy/friendly-intro-to-differential-privacy.html)

## Existing github repos about DP
- [Billy1900/Awesome-Differential-Privacy](https://github.com/Billy1900/Awesome-Differential-Privacy)
- [menisadi/awesome-differential-privacy](https://github.com/menisadi/awesome-differential-privacy)

---

Please cite this post using either this `BibTeX` entry
```
@misc{wang2023awesome,
  title   = "Awesome Differential Privacy for Statisticians",
  author  = "Wang, Zhanyu",
  year    = "2023",
  howpublished = "\url{https://github.com/Zhanyu-Wang/Awesome-Differential-Privacy-for-Statisticians/blob/main/README.md}"
}
```
or just

`Zhanyu Wang. Awesome differential privacy for statisticians. https://github.com/Zhanyu-Wang/Awesome-Differential-Privacy-for-Statisticians/blob/main/README.md, 2023.`

