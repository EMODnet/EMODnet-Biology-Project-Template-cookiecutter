# EMODnet Biology Project Template

This repository contains a template for developing data products in the framework of [EMODnet Biology](https://www.emodnet-biology.eu/).

## Directory structure

```
{{cookiecutter.directory_name}}/
├── analysis
├── data/
│   ├── derived_data/
│   └── raw_data/
│   	└── data.csv
├── docs/
├── product/
└── scripts/
```

* **analysis** - R Markdown or Jupyter Notebooks
* **data** - Raw and derived data. The original raw data must not be modified.
* **docs** - Rendered reports
* **product** - Output product files
* **scripts** - Reusable code

## Getting started

To start a project using this template, you need to install [cookiecutter](https://github.com/cookiecutter/cookiecutter) first. Run the following statement in the command line to create a new project.

```bash
$ cookiecutter https://github.com/EMODnet/EMODnet-Biology-Project-Template-cookiecutter
```

Alternatively, you can fork this repository https://github.com/EMODnet/EMODnet-Biology-Project-Template. You will have to replace the {{tags}} manually in the README, and download the data from EMODnet Biology into the `raw_data` directory. The content of these tags is described below.

## Sections

The README.md file of your project will include the sections described below:

* **Introduction:** Basic introduction to the product. Tags involved: *{{product_name}}* and *{{product_introduction}}*, 
* **Data series**: Some info about where the data comes from, or the different datasets that are combined. Tags involved: *{{data_series}}* and *{{data_wfs_request}}*
* **Data product**: What is the resulting data product (including images/graph), what can be concluded? What are the main findings?. Tags involved: *{{data_product_description}}*
* **More information:**
	* **References**: (optional) Add here the citations you may include in your explanation.
	* **Code and methodology**: Link to code/github. Tags involved: *{{link_code}}*
	* **Citation and download link**: how should this product be cited? Tags involved: *{{product_citation}}* and *{{link_download}}*
	* **Authors**: who contributed to the product?. Tags involved: *{{product_authors}}*

## Tags

This template will ask for the following input:

* **directory_name:** The name of the new directory containing the project. This name must consist of the syntax *"EMODnet-Biology-"* followed by the name or acronym of your project without spaces nor special characters. An example would be "EMODnet-Biology-zooplankton-abundance"

* **product_name:** The name of the project in plain text. This will be added to the README.md file. For example "Ecological niche model of zooplankton abundance"

* **product_introduction**: A short description about the project. It will be added to the README.md file.

* **product_authors:** Who contributed to the product?

* **product_citation:**  How this product should be cited?

* **data_series:** A description about where the data came from, or different datasets that were combined.

* **data_wfs_request:** If the data was downloaded from EMODnet Biology, provide here the WFS request. You can use the [download toolbox](https://www.emodnet-biology.eu/toolbox/en/download/occurrence/explore) to select the desired data. Once your query is ready, click on "Get webservice url" and paste the link here. The data will be downloaded on ~/data/raw_data/. ![toolbox](https://github.com/EMODnet/EMODnet-Biology-Project-Template-cookiecutter/blob/master/toolbox_screenshot.png)

  This tag only accepts to WFS requests in CSV format. If you used other sources of data with webservices available, please add these requests in the data series section.

* **data_product_description**: Describe here your results and your main findings.

* **link_download**: Provide here the link where your product is available to download

* **link_code:** Add a link to the repository where the code used to create your product is stored.

## Contact
Please feel free to write some lines to [bio@emodnet.eu](mailto:bio@emodnet.eu) if you have any questions.
