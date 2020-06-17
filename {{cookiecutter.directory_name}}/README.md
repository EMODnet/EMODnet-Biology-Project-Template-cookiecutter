# {{cookiecutter.product_name}}

## Introduction

{{cookiecutter.product_introduction}}

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

* **analysis** - Markdown or Jupyter notebooks
* **data** - Raw and derived data
* **docs** - Rendered reports
* **product** - Output product files
* **scripts** - Reusable code

## Data series

{{cookiecutter.data_series}}

```
{{cookiecutter.data_wfs_request}}
```

## Data product

{{cookiecutter.data_product_description}}

## More information:

### References

### Code and methodology

{{cookiecutter.link_code}}

### Citation and download link

This product should be cited as:

{{cookiecutter.product_citation}}

Available to download in:

{{cookiecutter.link_download}}

### Authors

{{cookiecutter.product_authors}}