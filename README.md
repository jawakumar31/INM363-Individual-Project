
# Building a Knowledge Graph from PDF files to query informations

Code for the final project analyzing and Building the Knowledge Graph



## Installation

Install all the necessary packages from requirements.txt

```bash
 pip install -r requirements.txt
```
    
## Acknowledgements

 - [PDFplumber](https://pypi.org/project/pdfplumber/0.1.2/)
 - [Spacy](https://spacy.io/models/en)
 - [Stanford OpenIE](https://github.com/philipperemy/stanford-openie-python)
 


## Pipeline

The jupyter notebook named KG_generator_fromPDF.ipynb is the main code for our project

This contains three main modules and an exploration sections of the Knowledge Graph.

All PDFs are stored under the "data/" folder from which the code reads and generates the Knowledge Graph out of it.


### Module 1 

This reads the PDF file and cleans it and reconstruct the text extracted mapped to its headings, titles and its contents

### Module 2 

This creates the triplets for the Knowledge Graphs.

Function 'custom_rules_triplets' creates triples based on custom rules for getting the subject-verb-object triples

In other method Stanford OpenIE is used to get the triplets

### Module 3

In here Graphs are created using PyViz libraries

HTML file of the grpah tool is stored in 'results/' folder

### Exploration

Node embeddings are created using node2vec library.

PCA code lets the user to project the embeddings in 2D space

