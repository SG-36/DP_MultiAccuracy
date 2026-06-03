# Differentially Private Multiaccuracy Boosting

Course project for CS 2260 (Differential Privacy) at Harvard University, advised by Professor Cynthia Dwork.

**Authors:** Suhwan Bong, Sarra Guezguez, Annabel Lowe

We extend the Multiaccuracy Boost algorithm (Kim et al., 2019) to satisfy (ε, δ)-differential 
privacy with respect to the audit dataset. The key contributions are:

- A DP-SGD auditor training procedure with formal per-round privacy guarantees
- A noisy correlation query using the Gaussian mechanism for the stopping condition
- Composition proofs showing the full boosting procedure is (ε, δ)-DP
- Empirical evaluation on the LFW dataset showing the privacy-fairness-accuracy tradeoff

## Results

DP-MA substantially reduces group accuracy gaps (e.g. from 0.071 to 0.010 for the Indian 
subgroup) at the cost of overall accuracy (~10 percentage point drop), consistent with the 
theoretical incompatibility between exact fairness and differential privacy.

## Reference

Kim, M. P., Ghorbani, A., & Zou, J. (2019). Multiaccuracy: Black-box post-processing for 
fairness in classification. AAAI/ACM Conference on AI, Ethics, and Society.

## Original codebase

# MultiAccuracyBoost
Multiaccuracy: Black-Box Post-Processing for Fairness in Classification

**Please cite the following work if you use this benchmark or the provided tools or implementations:**

```
@inproceedings{kim2019multiaccuracy,
  title={Multiaccuracy: Black-box post-processing for fairness in classification},
  author={Kim, Michael P and Ghorbani, Amirata and Zou, James},
  booktitle={Proceedings of the 2019 AAAI/ACM Conference on AI, Ethics, and Society},
  pages={247--254},
  year={2019},
  organization={ACM}
}
```
## Getting Started
Here is the tensorflow implementations of the paper [Multiaccuracy: Black-Box Post-Processing for Fairness in Classification](https://arxiv.org/abs/1805.12317) presented at NeurIPS 2019.

### Prerequisites

Required python libraries:

```
  Scikit-learn: https://scikit-learn.org/stable/
  Tensorflow: https://www.tensorflow.org/
  Facenet: https://github.com/davidsandberg/facenet
```
Also the LFW+A dataset images.

### Installing

Dowanload LFW+A dataset images and put them in a "./LFWA+/lfw" directory. "dataset_description.pkl" maps each image's name to its attributes.

## Authors

* **Michael P. Kim** - [Website](https://cs.stanford.edu/~mpkim/)
* **Amirata Ghorbani** - [Website](http://web.stanford.edu/~amiratag)
* **James Zou** - [Website](https://sites.google.com/site/jamesyzou/)


## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
