# COMP433 Project
- **[High level description/presentation of the project]**
---
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
- ### **[`keras`](https://keras.io/getting_started/)**
    - **Note:** This project uses pytorch as the backend for keras. When installing keras, **you may have trouble trying to change the backend** as it tries to find the `tensorflow` module when importing. Find the `keras.config` file (usually stored in `~/Users/{username}/.keras`) and change the `backend` property to `"torch"`, and then restart the notebook runtime.
    - [Setup Aid](https://keras.io/getting_started/intro_to_keras_for_engineers/)
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
- **[Instruction on how to train/validate your model]**
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
