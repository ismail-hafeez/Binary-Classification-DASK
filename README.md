# Parallel & Distributed Computing (PDC) Semester Project

## Project Overview
This project applies binary classification to a dataset of 41,000 records and 8 original features, aiming to:
1. Achieve baseline classification metrics (Accuracy, F1 Score, Confusion Matrix).  
2. Leverage parallel/distributed computing (Dask) to reduce model training time by ≥70%.

---

## Tech Stack
- **Language:** Python 3.10+  
- **Libraries:**
  - Data manipulation: `pandas`, `numpy`  
  - Visualization: `matplotlib`, `seaborn`  
  - Modeling: `scikit-learn`, `xgboost`, `imbalanced-learn (SMOTE)`  
  - Parallelism: `dask`, `dask-ml`  
- **IDE:** Visual Studio Code  
- **OS:** Ubuntu 24.04 LTS  

---

### Create a virtual environment & install dependencies
```
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Data Preprocessing
1. **Missing Values**  
   
2. **Categorical Encoding**  
  
3. **Train/Test Split**  
  
4. **Imbalance Handling**  
   
## Feature Engineering
---

### Parallel Model (Dask)
## Cluster Setup
from dask.distributed import Client, LocalCluster
from dask_ml.wrappers import ParallelPostFit

cluster = LocalCluster()
client = Client(cluster)

Results
Model	Accuracy	            F1 Score	Time (s)	Speed-Up

Random Forest (sequential)	0.5898	  0.3078	  17.97	–

Random Forest (Dask)	      0.5898	  0.3078	  2.14	≈ 88% faster


