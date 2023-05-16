# ipy_JSME_SMARTS-pattern-search
A Jupyter notebook that allow user to draw a molecule and highlight substructure of interest.

## Launch with binder
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/molmdl/ipy_JSME_SMARTS-pattern-search.git/main?urlpath=https%3A%2F%2Fgithub.com%2Fmolmdl%2Fipy_JSME_SMARTS-pattern-search%2Fblob%2Fmain%2FJSME_custom_SMARTS_highlight.ipynb)
Takes some time to load. Retry if you get an error. Jupyter Lab is not working, switch to classic via the upper menu bar ‘Help’ > ‘Launch Classic Notebook’. 

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

Majority of the codes were taken from the following resources:
1. <a href="https://github.com/lithium0003/JSME_ipywidget">JSME_ipywidget</a>
2. "T003_compound_unwanted_substructures" of <a href="https://github.com/volkamerlab/teachopencadd">TeachOpenCADD</a> 

Reference:
1. (a)<a href="https://jsme-editor.github.io/">JSME editor</a> (b) <a href="https://github.com/lithium0003/JSME_ipywidget">JSME_ipywidget for jupyter notebook</a>
2. <a href="https://www.rdkit.org">RDKit official website</a>
3. teachopencadd talktorials (a) Publication <a href="https://jcheminf.biomedcentral.com/articles/10.1186/s13321-019-0351-x">[1]</a> <a href="https://doi.org/10.1093/nar/gkac267">[2]</a>, (b) <a href="https://projects.volkamerlab.org/teachopencadd/">website</a>, (c) <a href="https://github.com/volkamerlab/teachopencadd">Github </a>
4. <a href="https://doi.org/10.1002/cmdc.200700139">The Brenk filter.</a> Actually its already implemented in RDKit, using it to test the use of custom filters.
