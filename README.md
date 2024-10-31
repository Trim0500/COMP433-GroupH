---
---

# COMP432 Project

---

## Authors
- ### **Tristan Lafleur (40245238)**
- ### **Nicholas Cook (40175800)**
- ### **Zaid Minhas (40243097)**
- ### **Marc-Laurent Frenette (40226091)**

---

### Required Libraries
- **[`pandas`](https://pandas.pydata.org/docs/index.html)**
- **[`matplotlib`](https://matplotlib.org/stable/users/getting_started/)**
- **[`numpy`](https://numpy.org/install/)**
- **[`torch`](https://pytorch.org/get-started/locally/)**
    - **Note:** You need to install the CUDA runtime in order to work with GPUs. Make sure to select the appropriate CUDA runtime, package manager and OS.
- **[`keras`](https://keras.io/getting_started/)**
    - **Note:** This project uses pytorch as the backend for keras. When installing keras, **you may have trouble trying to change the backend** as it tries to find the `tensorflow` module when importing. Find the `keras.config` file (usually stored in `~/Users/{username}/.keras`) and change the `backend` property to `"torch"`, and then restart the notebook runtime.
    - [Setup Aid](https://keras.io/getting_started/intro_to_keras_for_engineers/)
- **[`keras_nlp`](https://keras.io/guides/keras_nlp/getting_started/)**

---

### Datasets
- **[Source Train Set](https://www.kaggle.com/competitions/contradictory-my-dear-watson/data?select=train.csv)**
- **[Source Test Set](https://www.kaggle.com/competitions/contradictory-my-dear-watson/data?select=test.csv)**
- Utilize the `[COMP433]_Generate_Datasets.ipynb` notebook to download and prepare the data

---

### Models Implementations
- **ELECTRA EN Model:** `[COMP433]_ELECTRA_EN_Model.ipynb`
    - **[Model Card](https://github.com/google-research/electra)**

---
---