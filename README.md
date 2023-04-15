# ASC-self-tuned-k

[![DOI](http://img.shields.io/badge/doi-10.1016/j.patrec.2019.02.006-36648B.svg)](https://doi.org/10.1016/j.patrec.2019.02.006)
[![Paper](http://img.shields.io/badge/arXiv-2302.11297-b31b1b.svg)](https://arxiv.org/abs/2302.11297)
[![Papers with Code](http://img.shields.io/badge/PaperswithCode-2302.11297-21cbce.svg)](https://paperswithcode.com/paper/approximate-spectral-clustering-with)

## 	Approximate spectral clustering with eigenvector selection and self-tuned k
This is an implementation for the following paper:
```bibtex
@article{ALSHAMMARI201931,
	title = {Approximate spectral clustering with eigenvector selection and self-tuned k},
	journal = {Pattern Recognition Letters},
	volume = {122},
	pages = {31-37},
	year = {2019},
	doi = {https://doi.org/10.1016/j.patrec.2019.02.006},
	author = {Mashaan Alshammari and Masahiro Takatsuka}
}
```

## How to use:

Run BATCH_Points.m which will execute the following:
1.	PRE_Points.m to load toy data, csv files are the groundtruth labels.
2.	RUN_Points.m to perform spectral clustering with 4 functions to estimate k:
	- CostEigenGap.m a conventional method to estimate k
	- CostZelnik.m uses the method proposed by (Zelnik-manor 2005) to estimate k
	- CostDBIOverLambda.m uses the method proposed by our paper to estimate k
	- CostDBIOverLambdaPCA.m a uses the method proposed by our paper to estimate k followed by PCA variance filtering
3.	POST_Points.m to compute the accuracy of clustering

---
Provided by Mashaan Alshammari<br/>
mashaan14 at gmail dot com<br/>
mashaan dot awad at outlook dot com<br/>
July 03, 2019.
