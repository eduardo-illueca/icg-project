# ICG_subcomplexes - Morphological Analysis of ICG Signals and Characteristic Point Delineation Algorithm

This folder contains the code developed by María as part of the Bachelor's Thesis project on the morphological grouping of Impedance Cardiography (ICG) signals. 
The work is framed within the broader `icg-project` repository and focuses specifically on identifying and characterizing ICG subcomplexes using unsupervised 
methods (clustering kemodoids). The results are compared with an Artificial Neural Network (ANN).

## Project organization

This subfolder includes **10 Colab notebooks** divided into two main blocks, each corresponding to a different ICG signal database:

### HeartCycle database

The following notebooks are included:

- **HC_raw_data.ipynb**  and **HC_filtered_data.ipynb**
  Visualization of raw and filtered signals of the HearCycle database.

- **HC_full_code_definitive_k=2.ipynb**  
  Unsupervised clustering of ICG segments into 2 morphological subtypes.

- **HC_full_code_definitive_k=3.ipynb**  
  Same methodology adapted to identify 3 subtypes.

- **HC_full_code_definitive_k=4.ipynb**  
  Extension to 4 subtypes.

- **HC_full_code_definitive_k=5.ipynb**  
  Final configuration identifying 5 morphological ICG subtypes.

These notebooks use datasets stored in a private Google Drive folder. Nevertheless, the data will be public and therefore it can be run once access is granted.

---

### ReBeatICG database

This dataset is publicly available through Zenodo and is directly downloaded within the notebooks. The same clustering and delineation pipeline is applied using 4 different configurations:

- **RBICG_full_code_definitive_k=2.ipynb**
- **RBICG_full_code_definitive_k=3.ipynb**
- **RBICG_full_code_definitive_k=4.ipynb**
- **RBICG_full_code_definitive_k=5.ipynb**


---

## Notes on execution

- Each notebook contains a first section titled **"Libraries"**, where all necessary libraries are imported or installed (e.g., `dtw-python`, `scikit-learn`, `tqdm`, `matplotlib`, etc.).  
- All notebooks are written to be run on Google Colab without additional setup.  
- The pipeline includes both unsupervised clustering (K-Medoids with DTW distance) and supervised (Artificial Neural Network).
- It has been developed a delineation algorithm for characteristic point detection.

---

## Data accessibility

- **ReBeatICG database:** Publicly available and downloaded automatically from Zenodo in the corresponding notebooks.
- **HeartCycle database:** Stored in a Google Drive folder that will be public. 

---

## Academic context

This code was developed in the context of the Bachelor's Thesis titled:  
**"Evaluation of Clustering and Neural Network Approaches for Morphological Analysis in Impedance Cardiography and Characteristic Points Delineation"**  
by **María Morant Aranda**, under the supervision of Prof. Eduardo Illueca and Fernando Seoane, 2025.

