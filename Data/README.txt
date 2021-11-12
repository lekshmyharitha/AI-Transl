Malayalam Visual Genome 1.0 Release Description
-----------------------------------------------
http://hdl.handle.net/11234/1-3533
Shantipriya Parida
Idiap Research Institute
Martigny, Switzerland

Ondrej Bojar
Charles University, Faculty of Mathematics and Physics,
Institute of Formal and Applied Linguistics (UFAL)
2021


Data 
------- 
Malayalam Visual Genome (MVG for short) 1.0 has similar goals as Hindi Visual
Genome (HVG) 1.1: to support the Malayalam language. Malayalam Visual Genome 1.0
is the first multi-modal dataset in Malayalam for machine translation and image
captioning. 

Malayalam Visual Genome 1.0 serves in "WAT 2021 Multi-Modal Machine Translation
Task".

Malayalam Visual Genome is a multimodal dataset consisting of text and images
suitable for English-to-Malayalam multimodal machine translation task and
multimodal research. We follow the same selection of short English segments
(captions) and the associated images from Visual Genome as HGV 1.1 has. For MVG,
we automatically translated these captions from English to Malayalam and
manually corrected them, taking the associated images into account.

The training set contains 29K segments. Further 1K and 1.6K segments are
provided in development and test sets, respectively, which follow the same
(random) sampling from the original Hindi Visual Genome.

A third test set is called ``challenge test set'' and consists of 1.4K segments.
The challenge test set was created for the WAT2019 multi-modal task by searching
for (particularly) ambiguous English words based on the embedding similarity and
manually selecting those where the image helps to resolve the ambiguity. The
surrounding words in the sentence however also often include sufficient cues to
identify the correct meaning of the ambiguous word. For MVG, we simply
translated the English side of the test sets to Malayalam, again utilizing
machine translation to speed up the process.

Dataset Formats 
---------------------- 
The multimodal dataset contains both text and images. 

The text parts of the dataset (train and test sets) are in simple tab-delimited
plain text files. 

All the text files have seven columns as follows: 
Column1 - image_id 
Column2 - X 
Column3 - Y 
Column4 - Width 
Column5 - Height 
Column6 - English Text 
Column7 - Malayalam Text

The image part contains the full images with the corresponding image_id as the
file name. The X, Y, Width and Height columns indicate the rectangular region in
the image described by the caption.

Data Statistics 
------------------- 
The statistics of the current release are given below.

Parallel Corpus Statistics 
---------------------------------

Dataset             	Segments      	English Words       	Malayalam Words
----------          	--------------	--------------------	-----------------
Train               	         28930	              143112	107126
Dev                 	           998	                4922	3619
Test                	          1595	                7853	5689
Challenge Test      	          1400	                8186	6044
--------------------	------------  	------------------  	------------------
Total               	         32923	              164073	122478

The word counts are approximate, prior to tokenization. 

Citation 
----------- 

If you use this corpus, please cite the following paper: 

@article{hindi-visual-genome:2019, title={{Hindi Visual Genome: A Dataset for Multimodal English-to-Hindi Machine Translation}}, author={Parida, Shantipriya and Bojar, Ond{\v{r}}ej and Dash, Satya Ranjan}, journal={Computaci{\'o}n y Sistemas}, volume={23}, number={4}, pages={1499--1505}, year={2019} }

English - Malayalam multimodel  translation system using 