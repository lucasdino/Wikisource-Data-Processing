# English Wikisource Dump 🧠

Data retrieved from [Wikimedia](https://wikimedia.bringyour.com/enwikisource/20240320/?C=S&O=D) as of March 20, 2024. This dump includes all pages and articles from the English Wikisource project.

The `process_wikisource.ipynb` is a processing script that walks through the various steps to convert the ~13GB unzipped XML file into a binary format optimized for machine learning workflows (Parquet). This conversion facilitates the use of PyTorch's `Dataset` and `DataLoader` classes for more efficient data handling in training applications.

---
### How To Use:
Download the zipped file from the above Wikimedia link. I used `enwikisource-20240320-pages-articles.xml.bz2`. Extract the XML file, and then in the `process_wikisource.ipynb` file, make sure to set the `path` variable to the extracted XML file. 

Then, you can quickly run through the various steps to visualize and tune your processing function before doing a mass processing job.