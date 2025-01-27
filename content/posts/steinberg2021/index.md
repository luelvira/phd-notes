+++
title = "Steinberg2021"
author = ["Steinberg", "Ethan and Jung", "Ken and Fries", "Jason A. and Corbin", "Conor K. and Pfohl", "Stephen R. and Shah", "Nigam H."]
date = 2025-01-22T12:04:00+01:00
draft = false
+++

## Language Models Are an Effective Representation Learning Technique for Electronic Health Record Data {#language-models-are-an-effective-representation-learning-technique-for-electronic-health-record-data}

The authors of this paper aim to determine how to represent patient
information records. To commit the task, they have performed a search for
different methodologies.

The first problem they highlight is defining the transformation of the records
into a fixed length representation is an expensive process because is a manual
work, time-consuming and task-dependent, leaving much of the data underutilized.

Also, using deep neural network could be appealing, but it has not demonstrate
better performance than count based method combined with logistic regression or
gradient boosted trees, as demonstrated Rajkomar et al (Rajkomar, Alvin and Oren, Eyal and Chen, Kai and Dai, Andrew M. and Hajaj, Nissan and Hardt, Michaela and Liu, Peter J. and Liu, Xiaobing and Marcus, Jake and Sun, Mimi and Sundberg, Patrik and Yee, Hector and Zhang, Kun and Zhang, Yi and Flores, Gerardo and Duggan, Gavin E. and Irvine, Jamie and Le, Quoc and Litsch, Kurt and Mossin, Alexander and Tansuwan, Justin and Wang, De and Wexler, James and Wilson, Jimbo and Ludwig, Dana and Volchenboum, Samuel L. and Chou, Katherine and Pearson, Michael and Madabushi, Srinivasan and Shah, Nigam H. and Butte, Atul J. and Howell, Michael D. and Cui, Claire and Corrado, Greg S. and Dean, Jeffrey, 2018) and
Chen et al. (Chen, David and Liu, Sijia and Kingsbury, Paul and Sohn, Sunghwan and Storlie, Curtis B. and Habermann, Elizabeth B. and Naessens, James M. and Larson, David W. and Liu, Hongfang, 2019). **The core hypothesis of this work posits that it is
possible to use data from a large numbers of patients to learn reusable,
fixed-length representations which in turn improve the accuracy of clinical prediction models
trained on smaller subset of patients.**

One technique wide used in Natural Language process (NLP) and Computer Vision
(CV) is the representation learning that consists of creating a superset of data
for the training process with a limited training data. Due to their
similarities, previous work on representation learning for EHR data has followed
advancements in NLP. It is possible to treat medical codes in the EHR as words and learn
representations for medical codes by adapting Word2Vec to deal with the lack of
ordering of medical codes within an encounter However Miotto et al.
(Miotto, Riccardo and Li, Li and Kidd, Brian A. and Dudley, Joel T., 2016) learned that patient level representation using autoencoders,
reporting significantly better performance. But Choi et al. (Choi, Edward and Bahadori, Mohammad Taha and Searles, Elizabeth and Coffey, Catherine and Thompson, Michael and Bost, James and Tejedor-Sojo, Javier and Sun, Jimeng, 2016)
found that stacked autoencoders have not better performance that other
baselines.

For the representation, they have chosen four categories:

1.  Count based representation: This is the simplest representation they
    considered. This consists on counts of each code in the EHRs. They also,
    evaluated two enhancements:
    1.  _Time binning_: counts occurrences of a code in different time buckets separately
    2.  _Ontology expansion_: is a commonly used technique to mitigate issues related
        to the high dimensionality and sparsity of the data.
2.  Word2Vec representation: This type of representation requires managing the
    unordered nature of codes  occurring in a given day.
3.  Latent Semantic Indexing Representatins: They use LSI to construct patient
    level representation by treating each patient's EHR as a document, and each
    code as  a word.
4.  Clinical Language Model Based Representations. The core idea is to represent
    the data in a format that a model which is able to predict sequences of
    symbols can interpreted and predict successfully. There are two steps:
    1.  Defining the language model.
    2.  Transferring the information from the learned language model.
