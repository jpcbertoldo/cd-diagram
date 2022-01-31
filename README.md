# Critical Difference Diagrams 

This repository is adapted from [hfawaz/cd-diagram](https://github.com/hfawaz/cd-diagram) (tnx, @hfawaz!).

It contains the necessary code to generate a critical difference diagram based on the Wilcoxon-Holm method to detect pairwise significance. 

## Result 

Run `python main.py --help` using Python 3 to see the options.

**Quick start**: `python main.py --file ./data/example.csv --output-dir ./figs` will generate a critical difference diagram with Wilcoxon-Holm post-hoc analysis for the data present in [data/example.csv (!!!!!!!!!!!!!!place url!!!!!!!!!!!)]().

![figs/cd-diagram-example](https://github.com/hfawaz/cd-diagram/blob/master/cd-diagram.png)

First the Friedman test is performed to reject the null hypothesis, we then proceed with a post-hoc analysis based on the Wilcoxon-Holm method. 
We can clearly see how on average ```clf3``` and ```clf5``` were the best algorithms over the 15 datasets. 
A thick horizontal line groups a set of classifiers that are not significantly different. 

## Requirements

To run this code you will need the following python packages: 

* [numpy](https://www.numpy.org/)
* [pandas](https://pandas.pydata.org/)
* [matplotlib](https://matplotlib.org/)
* [scipy](https://www.scipy.org/)
* [networkx](https://networkx.github.io/)

## Reference 

This repo is just my touch to make the script more flexible and nice to use, the real authors is @hfawaz, who wrote [hfawaz/cd-diagram](https://github.com/hfawaz/cd-diagram).

As demanded in his repo, if you re-use this work, please cite:

```
@article{IsmailFawaz2018deep,
  Title                    = {Deep learning for time series classification: a review},
  Author                   = {Ismail Fawaz, Hassan and Forestier, Germain and Weber, Jonathan and Idoumghar, Lhassane and Muller, Pierre-Alain},
  journal                  = {Data Mining and Knowledge Discovery},
  Year                     = {2019},
  volume                   = {33},
  number                   = {4},
  pages                    = {917--963},
}
```
