# Awesome-Differential-Privacy-for-Statisticians

## What is special about 'DP for STAT'?
1. Knowledge about the population instead of the sample. 
2. Quantification of uncertainty from various sources. 
3. Art of the tradeoff between utility and privacy. 

---

## Intro for beginners
- [Why differential privacy is awesome](https://desfontain.es/privacy/differential-privacy-awesomeness.html)
- [Differential Privacy: An Introduction for First Graders](https://www.dataversity.net/differential-privacy-an-introduction-for-first-graders/#)

## What are the privacy issues when not using DP?
- [Potential privacy lapse found in Americans’ 2010 census data - AP News](https://apnews.com/article/aba8e57c145047b5bab11b62baaa7f7a)
- [Poking Holes in Genetic Privacy - The New York Times](https://www.nytimes.com/2013/06/18/science/poking-holes-in-the-privacy-of-dna.html)
- [NetFlix Cancels Recommendation Contest After Privacy Lawsuit](https://www.wired.com/2010/03/netflix-cancels-contest/)
- [Your Data Were ‘Anonymized’? These Scientists Can Still Identify You](https://www.nytimes.com/2019/07/23/health/data-privacy-protection.html)

Maybe it is necessary to emphasize: [Statistical Inference is Not a Privacy Violation](https://differentialprivacy.org/inference-is-not-a-privacy-violation/)

## Who are using DP?
- [US Census](https://www.nytimes.com/2018/12/05/upshot/to-reduce-privacy-risks-the-census-plans-to-report-less-accurate-data.html)
- [Google](https://static.googleusercontent.com/media/research.google.com/de//pubs/archive/42852.pdf), [Apple](https://docs-assets.developer.apple.com/ml-research/papers/learning-with-privacy-at-scale.pdf), [Microsoft](https://blogs.microsoft.com/ai-for-business/differential-privacy/), [Facebook](https://research.facebook.com/blog/2020/06/protecting-privacy-in-facebook-mobility-data-during-the-covid-19-response/), [Amazon](https://github.com/awslabs/sagemaker-privacy-for-nlp), [Snapchat](https://eng.snap.com/device-distributed-machine-learning), [Uber](https://www.wired.com/story/uber-privacy-elastic-sensitivity/), etc.

## Statisticians' slides
- Vishesh Karwa. [Differential Privacy and Statistical Inference: A statistician’s perspective](https://simons.berkeley.edu/sites/default/files/docs/6713/karwa-statisticalinferenceandprivacy.pdf)
- Aleksandra Slavković. [Differentially Private Estimators & Basic Statistical Inference](http://helper.ipam.ucla.edu/publications/data2010/data2010_8553.pdf)
- John C. Duchi. [Local Privacy, Statistical Minimax Rates, and Learning](https://web.stanford.edu/~jduchi/projects/DuchiJoWa13_talk.pdf)

---

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
