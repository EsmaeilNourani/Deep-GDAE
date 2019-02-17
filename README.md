# Deep-GDAE
Gene-Disease Association Extraction

Deep-GDAE integrates the specificities of a Convolution Neural Network (CNN) and an Attention-based Bidirectional Long Short-Term Memory Network to classify Gene-Disease Associations.


## Execution

W use several benchmark datasets to verify the performance.

1.[[Befree](https://www.ncbi.nlm.nih.gov/pubmed/25886734 "Extraction of relations between genes and diseases from text and large-scale data analysis")].

+ [`preProcess.ipynb`](Befree_GAD/pre_process.ipynb) Reads the data set and creates the primitive features including word and position embeddings, and saves the required file for training as a pickle file.

+ [`BeFree-3class.ipynb`](Befree_GAD/BeFree-3class.ipynb) Evaluation on the Genetic Association Database (GAD) : GAD is an archive of human genetic association studies of complex diseases and disorders. 

+ [`BeFree-2class_EUADR.ipynb`](Befree_EUADR/BeFree-2class_EUADR.ipynb) Evaluation on the EU-ADR dataset. It contains annotations on drugs, diseases, genes and proteins, and associations between them. Here we focus on gene disease associations.  

2.[[SNPPhenA corpus](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5383945/ "corpus for extracting ranked associations of single-nucleotide polymorphisms and phenotypes from literature")] corpus for extracting ranked associations of single-nucleotide polymorphisms and phenotypes from literature. 

The notebooks are executed as follows:

+ 1. Befree 

+ [`utils.ipynb`](utils.ipynb) contains the required methods which are called by other notebooks

+ [`Befree.ipynb`](Befree.ipynb) Evaluation using the BeFree corpus 

+ [`SNP.ipynb`](snp.ipynb) Results of prforming Deep-GDAE on the SNPPhenA corpus, which was developed with the purpose of extracting the ranked associations of SNPs and phenotypes from GWA studies. 

+ [`newCorpus.ipynb`](newCorpus.ipynb) Evaluation using the generated corpus

# Pre-trained word embedding models
Links for the word embedding models are provided below. The paths to theses models are added to the relavant notebooks.

+ PubMed-shuffle-win-30:
https://github.com/cambridgeltl/BioNLP-2016

+ Fast Text (crawl-300d-2M):
https://fasttext.cc/docs/en/english-vectors.html

+ PubMed w2v:
http://jbjorne.github.io/TEES/



