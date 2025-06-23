## 🧠 OMAMA: Oregon-Massachusetts Mammography Analysis Project

The **OMAMA project** is a collaborative research initiative focused on advancing automated cancer detection from mammography images using deep learning. Leveraging the **Chimera12 mammography archive**, this project aims to build a more structured and clinically usable dataset from raw hospital exports and evaluate the diagnostic power of different image-view combinations.

### 🧪 Objective

To scientifically evaluate and compare the effectiveness of using **single-view** vs **multi-view** mammographic images in cancer classification models. The study also involves building a clean dataset from semi-structured hospital exports and training classifiers to benchmark against the existing DeepSight tool.


### 📊 Key Components

* **Data Preparation**:

  * Raw DICOM and processed PNG images from the CHIMEA12 dataset.
  * Mapping metadata from associated CSVs and folder structures.
  * Organized patient-level image sets with labels for BI-RADS and pathology.

* **Experiments**:

  1. **View Combination Study**:

     * Compare DeepSight predictions using single-view (e.g., LCC, LMLO) vs all 4 views (LCC, LMLO, RCC, RMLO).
     * Wrapper script logs results, mismatches, and performance consistency.
  2. **Custom Classifier Development**:

     * Built and trained image classifiers using **DenseNet121**, **ResNet50**, and **U-Net**.
     * Evaluated using metrics like **accuracy**, **AUC**, and **IoU**.
  3. **CLI vs API Performance**:

     * Benchmarked inference time and output accuracy between command-line and web API-based model deployments.


### 🧰 Tools & Technologies

* Python, NumPy, Pandas, Matplotlib, Scikit-learn
* TensorFlow, Keras, PyTorch
* DICOM handling 
* DeepSight (open-source classifier wrapper)
* Custom wrapper scripts and dataset reformatting logic
* Linux CLI for distributed processing and performance testing


### 📈 Outcomes

* Creating a structured and reusable version of the mammography dataset for future researchers.
* Found notable variations in prediction quality between single and combined views.
* Proposed a lightweight benchmark pipeline for evaluating future classifiers.


### 🤝 Collaborators

* Jyostna Sree Somisetty (UMass Boston, MSIT)
* Prof. Daniel Haehn (UMass Boston, Research Advisor)
* Avanith Reddy (Research Partner)

### 📎 Related Datasets

* https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/KXJCIU
