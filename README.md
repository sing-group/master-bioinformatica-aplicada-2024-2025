# Machine Learning in Bioinformatics
> Máster en Bioinformática Aplicada a Medicina Personalizada y Salud (Curso 2024-2025)

# Scheduling

## First week (24-28 February 2025)
- Day 1 (24.02.2025) [*online*]:
  - 2/3 Theory
  - 1/3 Project: Session I ([project](PROJECT.md) presentation)
- Day 2 (25.02.2025) [*online*]:
  - 1/2 Theory
  - 1/2 Project: Session II
- Day 3 (26.02.2025) [*online*]: 
  - 2/3 Theory
  - 1/3 Project: Session III (with problem and dataset presentation [HITO-1](PROJECT.md))
- Day 4 (27.02.2025):
  - Practice: Hands-On (Machine Learning Basics in Python with scikit-learn Part I)
- Day 5 (28.02.2025):
  - 2/3 Practice: Hands-On (Machine Learning Basics in Python with scikit-learn Part II)
  - 1/3 Practical tips for Machine Learning

## Second week (3-5 February 2025)
- Day 6 (03.03.2025):
  - 1/2 Theory: presentation of a real case-study (the [PolyDeep project](https://polydeep.org/))
  - 1/2 Project: Session IV
- Day 7 (04.03.2025):
    - Project: Session III
- Day 8 (05.03.2025):
    - Project Session: IV (with results presentation [HITO-2](PROJECT.md))

# Practice

## Install Conda in your system

Download and install Miniconda from: https://www.anaconda.com/download/success

## Creating the Conda environment

Run the following command to create the Conda environment for the hands-on practice sessions:

```bash
conda env create -f environment.yml
```

And then activate it by running:
```bash
conda activate machine-learning
```

## Download the breast cancer dataset

During the hands-on sessions (Machine Learning Basics in Python with scikit-learn), we are going to use the `Breast Cancer Data` available [here](data/wdbc.data).

 This file came from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+(Diagnostic)). More information about this dataset can be found [here](https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wdbc.names) and [here](https://www.kaggle.com/uciml/breast-cancer-wisconsin-data).

To download it again, run the following commands: 
```bash
mkdir data

wget https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wdbc.data -O data/wdbc.data

sed -i '1iid,diagnosis,radius_mean,texture_mean,perimeter_mean,area_mean,smoothness_mean,compactness_mean,concavity_mean,concave points_mean,symmetry_mean,fractal_dimension_mean,radius_se,texture_se,perimeter_se,area_se,smoothness_se,compactness_se,concavity_se,concave_points_se,symmetry_se,fractal_dimension_se,radius_worst,texture_worst,perimeter_worst,area_worst,smoothness_worst,compactness_worst,concavity_worst,concave points_worst,symmetry_worst,fractal_dimension_worst' data/wdbc.data
```

# Project

The information about the project is available [here](PROJECT.md).

# References
- [Practical Statistics for Data Scientists: 50 Essential Concepts](https://www.oreilly.com/library/view/practical-statistics-for/9781491952955/)
- [Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow, 2nd Edition](https://www.oreilly.com/library/view/hands-on-machine-learning/9781492032632/)

# Additional Resources

## Papers
- Ten quick tips for machine learning in computational biology [[10.1186/s13040-017-0155-3](https://dx.doi.org/10.1186%2Fs13040-017-0155-3)]
- DOME: recommendations for supervised machine learning validation in biology [[10.1038/s41592-021-01205-4](https://doi.org/10.1038/s41592-021-01205-4)]
- The ABC recommendations for validation of supervised machine learning results in biomedical sciences [[10.3389/fdata.2022.979465](https://doi.org/10.3389/fdata.2022.979465)]

## Libraries
- [scikit-learn: machine learning in Python](https://scikit-learn.org/stable/)
- [Imbalanced-learn](https://imbalanced-learn.org/stable/index.html)
- [XGBoost](https://xgboost.readthedocs.io/en/stable/)
- [LIBSVM -- A Library for Support Vector Machines](https://www.csie.ntu.edu.tw/~cjlin/libsvm/)
