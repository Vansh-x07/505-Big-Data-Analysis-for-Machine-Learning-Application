# DS-505: Big Data Handling and Management for Machine Learning Applications

Practical assignment code for **B.Sc. (Data Science & Analytics), Semester V**, Academic Year 2026-2027.
Each practical is a self-contained Jupyter notebook holding the problem statement, the Python code and its execution output.

## Practicals

| # | Notebook | Unit |
|---|----------|------|
| 01 | [Dataset Ingestion, Inspection & Descriptive Statistics with Pandas](Practical_01_Dataset_Ingestion_Inspection_Descriptive_Statistics_with_Pandas.ipynb) | UNIT 1: Introduction to Big Data and Large Dataset Handling |
| 02 | [Data Hygiene: Missing Value Imputation, Deduplication & Renaming](Practical_02_Data_Hygiene_Missing_Value_Imputation_Deduplication_Renaming.ipynb) | UNIT 1: Introduction to Big Data and Large Dataset Handling |
| 03 | [In-Memory Optimization via Dtype Downcasting & Deep Profiling](Practical_03_In_Memory_Optimization_via_Dtype_Downcasting_Deep_Profiling.ipynb) | UNIT 1: Introduction to Big Data and Large Dataset Handling |
| 04 | [Out-of-Core Batch Ingestion & Aggregation via Chunking](Practical_04_Out_of_Core_Batch_Ingestion_Aggregation_via_Chunking.ipynb) | UNIT 1: Introduction to Big Data and Large Dataset Handling |
| 05 | [Apache Spark Session Initialization & DataFrame Schema Inspection](Practical_05_Apache_Spark_Session_Initialization_DataFrame_Schema_Inspection.ipynb) | UNIT 2: Big Data Processing using PySpark |
| 06 | [PySpark DataFrame Transformations: Selection, Filtering & Columns](Practical_06_PySpark_DataFrame_Transformations_Selection_Filtering_Columns.ipynb) | UNIT 2: Big Data Processing using PySpark |
| 07 | [Grouped Aggregations & Action Execution in PySpark](Practical_07_Grouped_Aggregations_Action_Execution_in_PySpark.ipynb) | UNIT 2: Big Data Processing using PySpark |
| 08 | [Columnar Storage with Apache Parquet Format in PySpark](Practical_08_Columnar_Storage_with_Apache_Parquet_Format_in_PySpark.ipynb) | UNIT 2: Big Data Processing using PySpark |
| 09 | [Missing Value Imputation with SimpleImputer & Categorical Encoding](Practical_09_Missing_Value_Imputation_with_SimpleImputer_Categorical_Encoding.ipynb) | UNIT 3: Preparing Big Data for Machine Learning |
| 10 | [Feature Scaling (StandardScaler vs MinMaxScaler) & Train-Test Split](Practical_10_Feature_Scaling_StandardScaler_vs_MinMaxScaler_Train_Test_Split.ipynb) | UNIT 3: Preparing Big Data for Machine Learning |
| 11 | [Continuous Predictive Modeling with Linear Regression](Practical_11_Continuous_Predictive_Modeling_with_Linear_Regression.ipynb) | UNIT 3: Preparing Big Data for Machine Learning |
| 12 | [Classification with Decision Trees & K-Nearest Neighbors (KNN)](Practical_12_Classification_with_Decision_Trees_K_Nearest_Neighbors_KNN.ipynb) | UNIT 3: Preparing Big Data for Machine Learning |
| 13 | [Text Data Cleaning & Custom Tokenization using Python](Practical_13_Text_Data_Cleaning_Custom_Tokenization_using_Python.ipynb) | UNIT 4: Introduction to Large Language Models and Big Data Applications |
| 14 | [Vocabulary Frequency Profiling & Stopword Filtering](Practical_14_Vocabulary_Frequency_Profiling_Stopword_Filtering.ipynb) | UNIT 4: Introduction to Large Language Models and Big Data Applications |
| 15 | [Pretrained Sentiment Analysis with Hugging Face Transformers](Practical_15_Pretrained_Sentiment_Analysis_with_Hugging_Face_Transformers.ipynb) | UNIT 4: Introduction to Large Language Models and Big Data Applications |
| 16 | [Automated Text Summarization using Pretrained LLM Pipeline](Practical_16_Automated_Text_Summarization_using_Pretrained_LLM_Pipeline.ipynb) | UNIT 4: Introduction to Large Language Models and Big Data Applications |

## Setup

```bash
git clone https://github.com/<your-username>/505-Big-Data-Analysis-for-Machine-Learning-Application.git
cd 505-Big-Data-Analysis-for-Machine-Learning-Application
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook
```

Then open any notebook and use **Run All**. You can also upload a notebook to Google Colab.

## Notes

- **Practicals 05-08 (PySpark)** need Java 17 or 21 installed (`java -version`). Spark runs locally, no cluster needed.
- **Practicals 15-16 (Hugging Face)** need an internet connection the first time, to download the pretrained models (about 270 MB and 1.2 GB). A free `HF_TOKEN` is optional and speeds up downloads.
- **Practical 04** writes a large temporary CSV and deletes it at the end.
- Datasets are generated inside each notebook with fixed random seeds, so results are reproducible and no external data files are required.
