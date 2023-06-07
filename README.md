<a href="http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0147596">
<img src="journal.pone.0176255.g002.png">
</a>

# Advancing machine learning for protein design, one dataset at a time 

## For machine learning research 

Benchmarks are the means by which we assess and improve machine learning algorithms. The goal of this repository is the creation of insanely difficult benchmarks in protein design. These benchmarks can be used to improve machine learning algorithms that seek to predict enzyme function. 


### Available benchmarks  

Currently, the primary dataset available is the Bagel dataset 

- Dataset name: Bagel 
- Samples: n=200 biophysically characterized designed enzymes 
- Targets: enzyme biophysical parameters k<sub>cat</sub>, K<sub>M</sub>, k<sub>cat</sub>/K<sub>M</sub>, and melting temperature (T<sub>m</sub>)

The goal for this benchmark set is to predict the enzyme kinetic constants (which span 7 orders of magnitude) from the sequence or any featurization of the input sequence. In our work, we featurize the protein sequences by means of molecular modeling. For each input sequence, we build a full-atom 3-D model of the protein–transition-state complex with molecular modeling software Rosetta, and use calculated structural features as input features to regularized linear models. [See our paper for our ability to predict kinetic constants](http://journals.plos.org/plosone/article?id=10.1371%2Fjournal.pone.0147596).


## For teachers 

### Investigating functional effects of mutations in a model enzyme to improve molecular modeling algorithms 

We are investigating how point mutations to enzymes change functional parameters, stabilty, and structure, and building a large data set of characterized variants to improve our ability to predict enzyme function with machine learning algorithms. This was a project in the Siegel Lab at UC Davis. Together, we designed and characterized the Michaelis-Menten kinetics and stability of mutants of a β-glucosidase (_BglB_, nicknamed "Bagel"). 

#### Oligo design and Kunkel mutagenesis

+ [A complete set of mutageneic oligos for the BglB gene](http://github.com/dacarlin/bagel-orders) is provided, but students should have the experience of either 1) writing the code to generate all possible oligos for the BglB sequence (see repository for data), or 2) designing an oligo "by hand" using DNA editing software 

+ there is a rough version of the Kunkel mutagenesis protocol in [the provided protocols](http://github.com/dacarlin/bagel-protocol), and a [more complete Kunkel protocol on the Siegel group website](https://drive.google.com/drive/folders/0B3zIXvOOrmpqcEM5WWRadThsVUE)


### For students

Welcome to the Bagel Team! You are expected to complete the following steps over the course of 3-6 months. 

#### 1. Background reading 

+ Paper that reported the [BglB crystal structure](http://www.sciencedirect.com/science/article/pii/S0022283607007413) in complex with a glycosyl intermediate  
+ [Our group's first paper on the BglB project](http://journals.plos.org/plosone/article?id=10.1371%2Fjournal.pone.0147596) describing the use of machine learning tools to make predictions based on the BglB data set 
+ [Our group's second paper on the BglB project](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0176255) assessing predictions of stability using different algorithms 

#### 2. Get started with using Foldit for protein design 

First, get a [our group's internal copy of Foldit](http://fold.it/dist/internal/build/). Then, download the [BglB Rosetta model](http://github.com/dacarlin/bagel-foldit), which comes with instructions for using Foldit. 

#### 3. Wet lab "boot camp" 

Get started in the wet lab by following the [protocols for protein production, purification, and kinetic assay](protocol/README.md) to produce, purify, and assay the BglB wild type protein, GFP, and two mutants. 

#### 4. Produce, purify, and assay your mutants in the wet lab

Following the procedures you learned in "boot camp", kinetically characterize the mutants that you designed. You will continue this step until your data is suitable for publication, as determined by the [data reporting guidelines](protocol/data_reporting_guidelines.md). 

#### 5. Analyze your data and learn from the mutations you designed

Analyze your data using the [data analysis tools](http://github.com/dacarlin/bagel-fitter) ([internal (UC Davis) link](http://bagel.genomecenter.ucdavis.edu) and write up your results. Learn how the mutations you made changed the kinetic properties of BglB.

#### 6. Design a second set of mutants that build on your ideas from the first set 

In this step, you form hypotheses based on your first round of mutants, and design a second round to test, expand, or refine those ideas. 

#### 7. Produce, purify, and assay your second round of mutants 

Following the procedures you learned in "boot camp", kinetically characterize the second round of mutants that you designed. 

#### 8. Analyze and compile your data 

Analyze your data using the [data analysis tools](http://github.com/dacarlin/bglb_fitter) ([internal (UC Davis) link](http://bagel.genomecenter.ucdavis.edu) and write up your results. For each mutant, the following should be reported (more in the data reporting guidelines) 

- a plot showing the mutant's kinetic data and Michaelis-Menten parameters 
- a plot showing the mutant's thermal data and T<sub>m</sub>
- an image of a gel band (with ladder) and assessments of expression (yes/no) and concentration of purified protein (reported in units of milligrams per liter) 

#### Write up your results for publication on BioArXiv

Write a short paper describing what you have found. 

