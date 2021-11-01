# Project Name



## How to use this repository?

This repository contains all info necessary to implement and reproduce the project/experiment

````
```
project
│   README.md
└───data
│    │   README.md
│    └───10-10-2021_Exp1
│    │    │   file1.fasta
│    │    │   file2.bed
│    │    │   ...
│		 │
│    └───shared
│      	  │   hg38.fasta
│         │   ...
│   
└───results
│    │   Results_Notebook.md
│    └───10-10-2021_Exp1
│   	    │   output1.bam
│   	    │   ...
│
└───doc
│    │    README.md
│    └───presentations
│    │    │   10-10-2021_Exp1.pptx
│ 	 │    │   ...
│		 │
│    └───notebooks
│    └───paper
│
└───src
     │   script.py
     │   code.R
```
````

`data/` : contains `README` file that contains instructions to obtain the input data and a copy of the input data. The input data folder should be named in a chronological order that matches the `results/` experiments folder. If some input data is shared between different experiments it should be stored in `data/shared/` directory. Some reference data (e.g. genom fasta file) might be in the parent workspace directory and this should be indicated in the `README` file, yet instructions to obtain and store them in `data/shared/` folder should be included as well.

`src/` : contains the source code and scripts used by all experiments in the project. If a source code is to be converted to a binary file, we can store it in `bin/` directory

`results/` : contains subfolders for each experiment conducted, named in a chronological order matching the naming convention in the `data/` directory. There is a `Results_Notebook` file that documents each experiments goals, results and remarks. Within each subfolder there is a `make` file to reproduce the whole experiment output along with scripts/notebooks for this specific experiment

`doc/` : contains the final documentation (powerpoint presentations, notebooks, papers, reports) of the project that will be shared with others to present the output. The documents are named with the corresponding experiment date in the `results/` directory. We may include a `README` file with the files correponding to different experiments.

* One should start with obtaining the data as indicated in the `data/` directory. Then you can implement different experiments (or start a new one) in the `results/` directory. If a script/code is used by more than once project it should be moved to `src/` . One can possibly start an experiment with a `draft` subdirectory within `results/` till the experiment is optimized. While crude goal, steps and findings are stored in the in the results notebook for authors documentation purposes, documentation for (possibly each) experiment should be written in `doc/` directory and referred to in the `Results_Notebook`. 
* Projects include necessary `git` files for version control. `.gitignore` files control what files/folders are pushed to GitHub



## Description of the project



## Links







