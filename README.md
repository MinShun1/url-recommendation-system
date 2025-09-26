# url-recommendation-system

This project builds a system that can recommend relevant URLs to users based on **popularity, tags, and temporal metadata** from the Delicious dataset. The system explores three machine learning approaches:  
1. **k-Nearest Neighbors (kNN)**  
2. **Neural Networks**  
3. **LightGBM**  

The system is based on **Content-Based Filtering**, recommending URLs by analyzing similarities between tags and metadata. To enhance performance and handle large scale data, **LightGBM** is used as a supervised model to predict URL relevance.

This project includes **data preprocessing**, **feature engineering**, and **evaluation of model performance**.

## Dataset
The dataset contains **99,983 popular URLs** bookmarked on the Delicious platform, with rich metadata capturing user behavior. Key features include:

- **URL** → the address of each bookmarked page (categorical).  
- **SaveCount** → total times a URL has been saved (numerical, indicates popularity).  
- **FirstSaveDate** → timestamp of first bookmark, transformed to extract year, month, and day (temporal features).  
- **Tags & Tag Counts** → up to 10 tags per URL (Tag1–Tag10, categorical) with counts (Count1–Count10, numerical) indicating tag relevance.  

The dataset spans from the late 1970s onward, allowing analysis of long-term trends in bookmarking activity and tag usage. It contains **23 columns** combining categorical, numerical, and temporal information suitable for content-based recommendation modeling.

## Repository Structure
- `1_Data/` → dataset used in this project.  
- `2_Notebook/` → Jupyter Notebook and HTML export of the code and analysis.  
- `3_Report/` → project report in PDF.
