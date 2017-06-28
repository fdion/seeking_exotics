# seeking_exotics

notebooks and related material from my data-intelligence.ai talk:

### Seeking Exotics: A Story of Visualization and Model Based Anomaly Detection

__Audience level__: Novice

__Topic area__: Misc

__Description__:

Medicare payments, UPC code descriptions, fertility rate and fires. All of it is data, some of which is erroneous and some of which is anomalous. Seeking Exotics introduces the audience to the world of outliers and anomaly detection through the use of metrics, visualizations and open source machine learning tools.

__Abstract__:

In 1777, Daniel Bernoulli wrote in his paper on the Most Likely Induction (maximum likelihood): "Is it right to hold
that the several observations are of the same weight or moment, or equally prone to any and every error?"
 
Ever since, mankind has been struggling as to what to do with erroneous and anomalous data. Finding them seems like 
a simple problem of clustering, and labeling them as such, like a simple problem of classification, but that would  
be oversimplifying the problem.

The "Seeking Exotics" talk will start with a light introduction to the world of outliers and anomaly detection. For 
more historical and background information, the audience is kindly invited to listen before the talk to 
[episode 2](http://artchiv.es/s4ym/posts/podcast-episode-002/) of the podcast "Something for Your Mind".

Through several sets of data covering various fields and types of data, several visualization techniques will be  
demonstrated. This will range from static box and stemgraphic plots to interactive mpld3 scatter plots. These will  
be combined with dimensionality reduction and clustering techniques (beyond PCA) in order to derive more insight  
from the data. 

Finally, one class classifiers (such as Isolation Forest) will do some heavy lifting for us with the  
easy to use scikit-learn giving us some results, ranging from sobering to surprising.

# After the fact

### The requirements

Besides installing Jupyter notebook and having Python 3.4 or greater (all of that installable through
[Anaconda](https://www.continuum.io/downloads), if you are new to python), you will need a few extra packages.

If you want to reproduce the results exactly as I demonstrated at the conference, here are the versions I used of each 
packages (_I had an incompatibility issue between seaborn and a more recent matplotlib_):

 - matplotlib==1.5.0
 - mpld3==0.3
 - numpy==1.12.0
 - pandas==0.19.2
 - scikit-learn==0.18.2
 - scikit-sos==0.1.10
 - scipy==0.18.1
 - git+https://github.com/mwaskom/seaborn.git
 - statsmodels==0.8.0
 - stemgraphic==0.3.6

Optionally, install python package _rise_ to use the slide deck presentation mode in Jupyter for the first two 
notebooks (that is how they were presented). Following is a breakdown of all of this by area.

### The building blocks

 - [numpy](http://numpy.org)
 - [pandas](http://pandas.pydata.org/pandas-docs/stable/)
 
 ### The statistical packages
 
 - [scipy.stats](https://docs.scipy.org/doc/scipy/reference/stats.html)
 - [statsmodels](http://www.statsmodels.org/stable/index.html)
 
### The machine learning
 
 - [scikit-learn](http://scikit-learn.org/)
 - [scikit-sos](https://github.com/jeroenjanssens/scikit-sos)
 - [lsanomaly](https://github.com/lsanomaly/lsanomaly)
 
### The visualization

 - [Matplotlib](http://matplotlib.org/)
 - [Seaborn](https://github.com/mwaskom/seaborn)
 - [Stemgraphic](http://stemgraphic.org)
 - [MPLD3](http://mpld3.github.io/)
 
See also:
 - [bokeh](http://bokeh.pydata.org)
 - [datashader](http://datashader.readthedocs.io/en/latest/)
 - [pygal](http://pygal.org)

### Learn more

During my talk, I brought up a few paper and book titles (the first 10). I also talked about a few more during the 
questions at the end (continuing over lunch time and the afternoon even). So for the benefit of many, here are some of 
them (_related to outliers, anomalies and visualization_):

 - Daniel Bernoulli, The Most Probable Choice Between Several Discrepant Observations and the Formation Therefrom of 
 the Most Likely Induction (1777), translated from latin by C. G. Allen, republished in Biometrika 48, 1 and 2 p.1 
 (1961) by M.G. Kendall
 - K.E. Basford and J.W. Tukey, Graphical Analysis of Multiresponse Data Illustrated With a Plant Breeding Trial 
 (1999), Chapman & Hall
 - J. W. Tukey, Exploratory Data Analysis (1977), Addison-Wesley
 - F. Dion, Stemgraphic a Stem-and-Leaf Plot for the Age of Big Data (2016)
 - P. J. Rousseeuw, A. M. Leroy, Robust Regression & Outlier Detection (1987), Wiley
 - W.J. Youdon, Experimentation and Measurement (1961), NIST special publication 672 
 - F. J. Anscombe, "Graphs in Statistical Analysis" (1973)
 - G. Lemaitre, F. Nogueira, C. K. Aridas, "Imbalanced-learn: A Python Toolbox to Tackle the Curse of Imbalanced 
 Datasets in Machine Learning" (2017), Journal of Machine Learning Research
 - F. T. Liu, K. M. Ting, "Isolation Forest" (2008), ACM
 - A. Cairo, The Functional Art an Introduction to Information Graphics and Visualization (2013), New Riders
 - E. J. Candes, X. Li, Y. Ma, J. Wright, "Robust Principal Component Analysis?" (2009), Journal of ACM 58, 1, p.1-37
 - M. Lima, Visual Complexity Mapping Patterns of Information (2011), Princeton Architectural Press
 - N. N. Taleb, Fooled by Randomness (2001), Random House
 - V. Barnett, T. Lewis, Outliers in Statistical Data (1978), Wiley
 - C. Aggarwal, Outlier Analysis (2013), Springer
 - D. Salzberg, The Lady Tasting Tea: How Statistics Revolutionized Science in the Twentieth Century (2001), Henry 
 Holt and Co
 - R. D. Cook, S. Weisberg, Residuals and Influence in Regression (1982), Chapman and Hall
 - M. Kantardzic, Data Mining Concepts, Models, Methods and Algorithms (2003), IEEE Press Wiley Interscience

### Further readings

And of course the various other publications I have listed in my "ex-libris" series on LinkedIn  
([part I](https://www.linkedin.com/pulse/ex-libris-data-scientist-part-i-francois-dion),
[part II](https://www.linkedin.com/pulse/ex-libris-data-scientist-part-ii-model-francois-dion), 
[part III](https://www.linkedin.com/pulse/ex-libris-data-scientist-part-iii-technology-francois-dion) and
[part IV](https://www.linkedin.com/pulse/ex-libris-data-scientist-part-iv-code-francois-dion) - part V on 
visualization and VI on communication are not yet available)
