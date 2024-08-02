
# Seoul Average Temperature Forecasting
___

## DACON competition : Seoul Average Temperature Forecasting
> **Competition** , **Mar. 2024 ~ May. 2024**

---

## Software Stacks
![](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)


---

## Competition Topic

Time Series Forecasting

Forecasting Seoul's average temperature from previous time series(temperature) data.

---

## Implementation

### 1. Dataset
- **Seoul Temperatures** : Average daily temperature data from 1960 to 2022

### 2. Data preprocessing

- Process "NULL" values
- Drop unusal features
  ![캡처](https://github.com/user-attachments/assets/1a8088d4-0eac-4f4e-8301-dc431f837c2c)


### 3. Model Selection
- Time Series Forecasting Model
- Tried method : ARIMA Model, Prophet ...
- **Patch Mixer** :: Gong, Zeying, Yujin Tang, and Junwei Liang. "Patchmixer: A patch-mixing architecture for long-term time series forecasting." arXiv preprint arXiv:2310.00655 (2023).
- code reference : [tsf-new-paper-taste : github](https://github.com/hughxx/tsf-new-paper-taste)

### 4. Hyperparameter
 - SEQ_LEN = 716
 - PATCH_LEN = 1
 - STRIDE = 2
 - EPOCHS = 100

---

## Result

- **Top 4%** , Mean absolute error 2.6186 (in private data)
  ![다운로드](https://github.com/user-attachments/assets/8afb256b-6899-4d97-beb7-f5097d689b0a)

