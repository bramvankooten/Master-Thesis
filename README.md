# Reference attribution in AI-powered voting guides
Bram van Kooten  
Master's Thesis in Computer Science  
Leiden Institute of Advanced Computer Science (LIACS)

## Data folder
The `data` folder consists of 15 files, one for each political party that was a part of this study. Each file contains a list of reference objects, which contain the `party`, `statement`, `summarySentence`, `paragraphs`, and true `references` for the given combination of political party and summarySentence. These are used to make predictions using 6 differenct methods.

## Predictions
In `data.ipynb` code is present to generate reference predictions for the 6 different methods. These can be found in the following methods: `handle_nli`, `handle_msmarco`, `handle_bm25`, `handle_e5`, and `handle_gpt` (`handle_gpt` is used for both GPT3.5 and GPT4). The predictions used for this thesis can be found in the `results` folder.

## Results
In the `results` folder, a json file can be found with predictions for each of the methods used. In `data.ipynb`, these files can be loaded in and used to perform the analysis used in the experiments of this thesis. The folder also includes `e5_embeddings.json`, which are the embeddings used by the E5 model, which further analysis is performed on. 