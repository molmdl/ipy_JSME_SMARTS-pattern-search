# ipy_JSME_SMARTS-pattern-search
A simple demo of using RDKit to highlight a custom set of substructures in a query molecule. List of substructures can be provided in a file uploaded by the user. Query molecule is drawn by the user via JSME.

[![License](https://img.shields.io/badge/License-BSD%203-lightgrey.svg)](https://opensource.org/license/bsd-3-clause/)
[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fgjbae1212%2Fhit-counter)](https://hits.seeyoufarm.com)                    

## Launch in BinderHub
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/molmdl/ipy_JSME_SMARTS-pattern-search.git/main?filepath=JSME_custom_SMARTS_highlight.ipynb)

- I haven't tried to optimize the binderhub config yet. It may or may not work. Better run it locally for stability.
- Takes some time to load. Retry may helps if you get an error. 
- If the above link is not working, try the following:
    - visit https://mybinder.org/v2/gh/molmdl/ipy_JSME_SMARTS-pattern-search.git/main
    - Switch to classic via the upper menu bar ‘Help’ > ‘Launch Classic Notebook’. 
    - launch JSME_custom_SMARTS_highlight.ipynb

## Install locally
1. Install <a href="https://www.anaconda.com/download/">Anaconda</a> or <a href="https://conda.io/miniconda.html">Miniconda</a>.
2. Clone this repository
>    git clone https://github.com/molmdl/ipy_JSME_SMARTS-pattern-search.git
3. cd to the cloned repository
>    cd ipy_JSME_SMARTS-pattern-search
4. Create a conda environment with required dependencies 
>    conda env create -f environment.yml
5. Activate the environment
>    conda activate ipy_JSME_SMARTS
6. Launch the notebook
>    jupyter notebook JSME_custom_SMARTS_highlight.ipynb

Workflow
1. Load the JSME editor and draw the molecule of interest
2. Upload the csv file containing the SMARTS pattern of your custom chemical filters.
3. Highlight the SMARTS pattern in the molecule drawn by the user.

Majority of the code was taken from the following resources:
1. <a href="https://github.com/lithium0003/JSME_ipywidget">JSME_ipywidget</a>
2. "T003_compound_unwanted_substructures" of <a href="https://github.com/volkamerlab/teachopencadd">TeachOpenCADD</a> 

Reference:
1. (a)<a href="https://jsme-editor.github.io/">JSME editor</a> (b) <a href="https://github.com/lithium0003/JSME_ipywidget">JSME_ipywidget for jupyter notebook</a>
2. <a href="https://www.rdkit.org">RDKit official website</a>
3. teachopencadd talktorials (a) Publication <a href="https://jcheminf.biomedcentral.com/articles/10.1186/s13321-019-0351-x">[1]</a> <a href="https://doi.org/10.1093/nar/gkac267">[2]</a>, (b) <a href="https://projects.volkamerlab.org/teachopencadd/">website</a>, (c) <a href="https://github.com/volkamerlab/teachopencadd">Github </a>
4. <a href="https://doi.org/10.1002/cmdc.200700139">The Brenk filter.</a> Actually its already implemented in RDKit, using it to test the use of custom filters.
