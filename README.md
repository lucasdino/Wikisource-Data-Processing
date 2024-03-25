# English Wikisource Dump 🧠

Data retrieved from [Wikimedia](https://wikimedia.bringyour.com/enwikisource/20240320/?C=S&O=D). This download source includes a large portion of the articles from the English Wikisource project (several million articles).

The `process_wikisource.ipynb` is a processing script that walks through the various steps to convert a large XML file into a binary format convenient for machine learning workflows (Parquet). For example, I used the March 20, 2024 download of *pages-articles* which has an unzipped XML file that is ~13GB. This conversion facilitates the use of PyTorch's `Dataset` and `DataLoader` classes for more efficient data handling in training applications.

---
### How To Use:
Download the zipped file from the above Wikimedia link. I used `enwikisource-20240320-pages-articles.xml.bz2`. Extract the XML file, and then in the `process_wikisource.ipynb` file, make sure to set the `path` variable to the extracted XML's filepath. 

Then, you can quickly run through the various steps to visualize and tune your processing function before doing a mass processing job.