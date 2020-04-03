# EphysExtraction
Code to extract electrophysiological parameters of neurons. Code is continuously being updated to handle more kinds of voltage traces and extract different kinds of features.

Development by: Yves Bernaerts (main)

Supervisor: Philipp Berens


Important folders: 
Script ephys_features.py contains basic functions to work with the raw voltage traces and extracts features. This is based on Allen Institute code also available on GitHub but the scripts have been modified.
Script ephys_extractor.py creates an object corresponding to one neuron/cell and extracts the electrophysiological properties based on features calculated by functions in extract_cell_features.py. This is also based on Allen Institute code available on GitHub but modified too.


The following jupyter notebooks are created to transform data given in a certain format to raw voltage traces. Electrophysiological features are extracted by calling to the two previously mentioned scripts and sanity checks are available by plotting the extracted information.


GetFeaturesPipeline.ipynb is finetuned to work with data from mini-atlas mouse motor cortex M1 (in collaboration with Andreas Tolias' lab (Houston)). It is advised to have a look at this pipeline when you consider to work with your own data.

Relatively outdated pipelines:
GetFeaturesPipeline2.ipynb is finetuned to work with data from Hippocampus (in collaboration with Xiaolong's lab (Houston))
GetFeaturesPipelineL4.ipynb is finetuned to work with data from layer 4 (V1 and S1) (in collaboration with Andreas Tolias' lab (Houston))
GetFeaturesPipelineL4Neurolucida.ipynb is finetuned to work with data from layer 4 V1 (in collaboration with Andreas Tolias' lab (Houston))

One can ask for permission to work with this data by contacting yves.bernaerts@uni-tuebingen.de

## Installation

In developer mode:
```shell script
git clone pip install git+https://github.com/berenslab/EphysExtraction
cd EphysExtraction
pip install -e .
```
