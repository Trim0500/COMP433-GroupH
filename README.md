# COMP433 Project

# Project Description

This project uses deep learning in natural language processing to solve a multilingual natural language inference task using transformer-based architectures. This task is the Kaggle challenge "Contradictory, My Dear Watson", which can be accessed here: https://www.kaggle.com/competitions/contradictory-my-dear-watson. The primary objective is to predict the logical relationship between pairs of sentences across multiple languages, categorizing them as entailment, contradiction, or neutrality.

We implemented and fine-tuned four transformer models for the NLI task:
- **BERT English:** Fine-tuned for sentence pairs in English.
- **BERT Multilingual:** Fine-tuned to handle sentence pairs across 15 languages.
- **ELECTRA English:** Fine-tuned for sentence pairs in English.
- **ELECTRA Multilingual:** Fine-tuned to handle sentence pairs across 15 languages.

## Results

### BERT Results
- **BERT English:** Achieved a test accuracy of 58% on the Kaggle dataset.
- **BERT Multilingual:** Outperformed BERT EN, achieving a test accuracy of 60%.

### ELECTRA Results
- **ELECTRA English:** Achieved a test accuracy of 59%.
- **ELECTRA Multilingual:** Achieved a test accuracy of 59%.

### Key Observations
- **Neutral Class Challenge:** Across all models, the neutral class was consistently misclassified. This issue is due to the lack of distinctive context in neutral sentences, making it harder for models to capture their semantic meaning.
- **Data Limitations:** The relatively small Kaggle dataset size limited model generalization.
---
## Authors
- ### **Tristan Lafleur (40245238)**
- ### **Nicholas Cook (40175800)**
- ### **Zaid Minhas (40243097)**
- ### **Marc-Laurent Frenette (40226091)**
---
---
### Required Libraries
- ### **[`pandas`](https://pandas.pydata.org/docs/index.html)**
- ### **[`matplotlib`](https://matplotlib.org/stable/users/getting_started/)**
- ### **[`numpy`](https://numpy.org/install/)**
- ### **[`sklearn`](https://scikit-learn.org/stable/install.html)**
- ### **[`keras`](https://keras.io/getting_started/)**
- ### **[`keras_nlp`](https://keras.io/guides/keras_nlp/getting_started/)**
- ### **[`keras-tuner`](https://keras.io/keras_tuner/getting_started/)**
---
---
### Google Colab 
- In order to open the notebooks and run the models, it is recommended to utilize [Google Colab](https://colab.research.google.com/).
    - Navigate to the "GitHub" section when opening notebooks and enter the repository URL to get a list of the available notebooks to select from.
    - When in a notebook, ensure that the runtime utilizes a GPU (i.e. L4, A100, T4, ...)
---
---
### Models Implementations
- **ELECTRA:** `[COMP433]_ELECTRA_EN_Model.ipynb` & `[COMP433]_ELECTRA_Multi_Model.ipynb`
    - **[Model Card](https://github.com/google-research/electra)**
- **BERT:** `[COMP433]_BERT_EN_MODEL.ipynb` & `[COMP433]_BERT_Multi_lingual_Model.ipynb`
    - **[Model Card](https://github.com/google-research/bert)**
---
---
### Model Weights
- [Google Drive Folder](https://drive.google.com/drive/folders/1FnHiWtmtQkssDtptO4cd9Zknub9hEn6H?usp=sharing)
---
---
### Training and Validating the Model
- Run the BERT [EN](https://github.com/Trim0500/COMP433-GroupH/blob/main/%5BCOMP433%5D_BERT_EN_MODEL.ipynb), [Multilingual](https://github.com/Trim0500/COMP433-GroupH/blob/main/%5BCOMP433%5D_BERT_Multi_lingual_Model.ipynb) or ELECTRA [EN](https://github.com/Trim0500/COMP433-GroupH/blob/main/%5BCOMP433%5D_ELECTRA_EN_Model.ipynb), [Multilingual](https://github.com/Trim0500/COMP433-GroupH/blob/main/%5BCOMP433%5D_ELECTRA_Multi_Model.ipynb) notebooks on [google collab](https://colab.research.google.com/).
- Ensure that the session runtime utilizes GPU.
- Ensure that the necassary [training dataset](https://github.com/Trim0500/COMP433-GroupH/tree/main/Datasets) .csv file is added to the running notebook's current work directory.
- EN models use _train_en.csv_ and Multilingual models use _train_all_languages.csv_.
- Weights found after training and after hyperparameter search tuning are both saved on collab session.
---
---
### How to Test the Pre-trained Models
- **[Instructions on how to run the pre-trained model on the provided sample test dataset]**
---
---
### Obtaining the Datasets
- **[Source Train Set](https://www.kaggle.com/competitions/contradictory-my-dear-watson/data?select=train.csv)**
- **[Source Test Set](https://www.kaggle.com/competitions/contradictory-my-dear-watson/data?select=test.csv)**
- Utilize the `[COMP433]_Generate_Datasets.ipynb` notebook to download and prepare the data
---
---
