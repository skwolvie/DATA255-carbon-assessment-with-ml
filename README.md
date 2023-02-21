## Carbon assessment with machine learning

This is the code repository accompanying the following paper published in WWW 2023 -- \
CaML: Carbon Footprinting of Household Products with Zero-Shot Semantic Text Similarity \
Bharathan Balaji, Venkata Sai Gargeya Vunnava, Geoffrey Guest, Jared Kramer

## Task: Automation of emission impact factor (EIF) mapping

We automate the process of mapping emission impact factors based on the text description of a product. This is one of the key steps in life cycle assessment. In a nutshell, we use a natural language model to identify an appropriate emission impact factor for a product description. 

Figure below gives an overview of the text similarity model inference.

<img src="images/sbert_model.png"  width="800">

## Installation
Required packages are given `requirements.txt`
Run the following commands to install the package:
```
git clone <repo>
cd carbon-assessment-with-ml
pip install -r requirements.txt
pip install -e .
```

## Getting Started
Follow the code in notebooks directory

## Dataset
The dataset consists of retail products mapped to North American Industry Classification System (NAICS) codes. The
mapping was done with Amazon Mechanical Turk, aggregating ground truth from 5 annotations per product. The dataset is the basis of estimating the carbon emissions of a product using Economic Input-Output Life Cycle Assessment (EIO-LCA). Dataset is stored as a Pandas
dataframe. 

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This project is licensed under the terms of the Apache 2.0 license. See `LICENSE`.
Included datasets are licensed under the terms of the CDLA Permissive license, version 2.0. See `LICENSE-DATA`.
