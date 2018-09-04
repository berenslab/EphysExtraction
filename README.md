# EphysExtraction
Code to extract electrophysiological parameters of neurons. Code is continuously being updated to handle more kinds of voltage traces.

Development by: Yves Bernaerts (main)
Supervisor: Philipp Berens


Important folders: 
Script extract_cell_features.py contains basic functions to work with the raw voltage traces and extracts features. This is based on Allen Institute code also available on GitHub but the scripts have been modified.
Script feature_extractor.py creates an object corresponding to one neuron/cell and extracts the electrophysiological properties based on features calculated by functions in extract_cell_features.py. This is also based on Allen Institute code available on GitHub but modified too.
GetFeaturesPipeline.ipynb is a jupyter notebook created to transform data given in a certain format to raw voltage traces. Electrophysiological features are extracted and sanity checks are available by plotting the extracted information.
