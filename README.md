# Deep-GDAE
Gene-Disease Association Extraction

Deep-GDAE integrates the specificities of a Convolution Neural Network (CNN) and an Attention-based Bidirectional Long Short-Term Memory Network to classify Gene-Disease Associations.

W use several benchmark datasets to verify the performance.

1.[[Befree](https://www.ncbi.nlm.nih.gov/pubmed/25886734 "Extraction of relations between genes and diseases from text and large-scale data analysis")].

+ Genetic Association Database (GAD) : GAD is an archive of human genetic association studies of complex diseases and disorders. 

+ EU-ADR dataset: The EU-ADR dataset contains annotations on drugs, diseases, genes and proteins, and associations between them 

2.[[SNPPhenA corpus](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5383945/ "corpus for extracting ranked associations of single-nucleotide polymorphisms and phenotypes from literature")] corpus for extracting ranked associations of single-nucleotide polymorphisms and phenotypes from literature. 

## Execution

The notebooks are executed as follows:

+ [`preProcess.ipynb`](pre_process.ipynb) reads the data set and creates the primitive features including word and position embeddings and save the required file for training as a pickle file.

+ [`utils.ipynb`](utils.ipynb) contains the required methods which are called by other notebooks

