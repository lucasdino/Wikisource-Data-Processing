# English Wikisource Dump
---
Data retrieved from [Wikimedia](https://wikimedia.bringyour.com/enwikisource/20240320/?C=S&O=D) as of March 20, 2024. This dump includes all pages and articles from the English Wikisource project./n
*process_wikisource.ipynb* is a processing script that walks through the various steps to convert the ~13GB unzipped XML file into into a binary format optimized for machine learning workflows (Parquet). This conversion facilitates the use of PyTorch's Dataset and DataLoader classes for more efficient data handling in training applications.