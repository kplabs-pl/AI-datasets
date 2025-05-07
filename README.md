# KP Labs Datasets 
<img src="kp.png" style="float: right;" />

At KP Labs, we promote and support the fair and transparent process of machine learning algorithms development in order to tackle the reproducibility crisis that we observe in (not only) satellite data analysis. Therefore, we release AI-ready datasets that can be used by the community. 

This page delivers links to the relevant repositories, dataset descriptions, as well as to the published scientific papers built upon the corresponding datasets.
If you feel that the dataset is useful for your research activities, it would be great if you could acknowledge and cite the corresponding works.

##### Jump to: [ESA-AD](#ESA-AD) (`AD`, `telemetry`), [OPSSAT-AD](#OPSSAT-AD) (`AD`, `telemetry`), [HYPERVIEW](#HYPERVIEW) (`EO`, `images`), [MuS2](#MuS2) (`SSR`, `images`)

# Anomaly detection in satellite telemetry data 

## ESA-AD
- ESA Anomaly Dataset (ESA-AD) is the first large-scale, real-life satellite telemetry dataset with curated anomaly annotations originated from three ESA missions. We hope that this unique dataset will allow researchers and scientists from academia, research institutes, national and international space agencies, and industry to benchmark anomaly detection models and approaches on a common baseline as well as research and develop novel, computational-efficient approaches for anomaly detection in satellite telemetry data.
  - metadata: `anomaly detection`, <kbd>timeseries</kbd>, `~12 GB`, `3 missions`, several years long telemetries, `CC-BY`
  - keywords: `machine learning`, `deep learning`, `unsupervised learning`, `supervised learning`, `European Space Agency`, `ESA`, `telemetry`, `signal processing`, `anomaly detection`
- DATA FILES: [DOI: 10.5281/zenodo.12528696](https://zenodo.org/records/12528696)
- CODE: [github.com/kplabs-pl/ESA-ADB](https://github.com/kplabs-pl/ESA-ADB)
- OFFICIAL KAGGLE CHALLENGE AND PREPROCESSED DATA: [https://www.kaggle.com/competitions/esa-adb-challenge](https://www.kaggle.com/competitions/esa-adb-challenge)

- DATASET PAPER: [Arxiv link](https://arxiv.org/abs/2406.17826), [BibTex file](bibtex/esaad.bib)
  - Kotowski. K., Haskamp, C., et al.: European Space Agency Benchmark for Anomaly Detection in Satellite Telemetry, 2024, ArXiv
    - _Highlights:_ processing and evaluation procedures description, with results of typical anomaly detection algorithms assessed in our novel hierarchical evaluation pipeline show that new approaches are necessary to address operators' needs using this dataset.
- PROJECT PAPER:
  - De Canio, G. et al. (2023) Development of an actionable AI roadmap for automating mission operations. In, 2023 SpaceOps Conference. American Institute of Aeronautics and Astronautics, Dubai, UAE.


## OPSSAT-AD
- OPSSAT Anomaly Dataset (OPSSAT-AD) contains the telemetry data acquired on board `OPS-SAT` - a CubeSat mission that has been operated by the European Space Agency. It is accompanied by the paper with baseline results obtained using 30 supervised and unsupervised classic and deep machine learning algorithms for anomaly detection. They were trained and validated using the training-test dataset split introduced in this work, and we present a suggested set of quality metrics that should always be calculated to confront the new algorithms for anomaly detection while exploiting OPSSAT-AD.
  - metadata: `anomaly detection`, `classification`, `outlier detection`, <kbd>timeseries</kbd> + <kbd>tabular</kbd>, `2134 samples`, `CC-BY`
  - keywords: `machine learning`, `deep learning`, `unsupervised learning`, `supervised learning`, `European Space Agency`, `ESA`, `telemetry`, `signal processing`, `anomaly detection`

- DATA FILES: [DOI: 10.5281/zenodo.12588359](https://zenodo.org/records/12588359)
- CODE: [github.com/kplabs-pl/OPS-SAT-AD](https://github.com/kplabs-pl/OPS-SAT-AD)

- DATASET PAPER: [Scientific Data](https://doi.org/10.1038/s41597-025-05035-3), [BibTex file](bibtex/opssat.bib)
  - Ruszczak, B., Kotowski. K., Evans, D., Nalepa, J.: The OPS-SAT benchmark for detecting anomalies in satellite telemetry, 2025, Scientific Data
    - _Highlights:_ delivers the baseline results for the unsupervised and supervised learning for the anomaly detection using this dataset,

- RESULTS PAPER: [ICCS 2023](https://doi.org/10.1007/978-3-031-35995-8_21), [BibTex file](bibtex/opssat-iccs.bib) 
  - Ruszczak, B., Kotowski. K., Andrzejewski, J., Nalepa, J., et al.: (2023). Machine Learning Detects Anomalies in OPS-SAT Telemetry. Computational Science – ICCS 2023. LNCS, vol 14073. Springer, https://doi.org/10.1007/978-3-031-35995-8_21
    - _Highlights:_ delivers the anomaly detection results, improved using the synthetic intermediate features generation and telemetry segments augmentation
 

# Earth observation

## HYPERVIEW
- The HYPERVIEW dataset was used in the HYPERVIEW Challenge organized at IEEE ICIP 2022 (Bordeaux, France), and further re-executed at AI4Good 2023.
This dataset targets the problem of estimating soil parameters from hyperspectral images, 
and it comprises 2886 hyperspectral images in total (2 m GSD), of which 1732 images are used for training and 1154 images for testing (the ground-truth labels, being in-situ measurements of the soil parameters, are not revealed for the test set). The hyperspectral image size varies (depending on agricultural parcels) and is on average around 60x60 pixels. Each patch contains 150 contiguous hyperspectral bands (462-942 nm, with a spectral resolution of 3.2 nm), which reflects the spectral range of the hyperspectral imaging sensor deployed on-board Intuition-1.
  - metadata: `HSI`, `2886` <kbd>hyperspectral images</kbd>, `2 m GSD`, `CC-BY` 
  - keywords: `regression`, `image processing`, `machine learning`, `deep learning`, <kbd>hyperspectral images</kbd>, <kbd>soil content analysis</kbd>, `macronutrients measurement`, `pH`, `P`, `K`, `Mg`, `satellites`, `hyperspectral imaging`, `benchmark testing`, `feature extraction`,
  - to calculate metrics and confront with the current state of the art, join the permanently open HYPERVIEW Challenge at https://platform.ai4eo.eu/seeing-beyond-the-visible-permanent 
- DATA AND CODE FILES: _HYPERVIEW Challenge_ (with its permanently open version available at https://platform.ai4eo.eu/seeing-beyond-the-visible-permanent)
- DATASET PAPER: [IEEE GRSM](https://doi.org/10.1109/MGRS.2024.3394040), [BibTex file](bibtex/hyper.bib)
  - Nalepa, J., Tulczyjew, L., Le Saux, B., Longépé, N., Ruszczak, B., Wijata, A. M., et al., "Estimating Soil Parameters From Hyperspectral Images: A benchmark dataset and the outcome of the HYPERVIEW challenge," in IEEE Geoscience and Remote Sensing Magazine, vol. 12, no. 3, pp. 35-63, Sept. 2024, https://doi.org/10.1109/MGRS.2024.3394040  
    - _Highlights:_ Apart from the detailed description of the AI-ready dataset, we present the top-performing teams (their detailed solutions and experimental results) from the HYPERVIEW Challenge. The solution developed by the winners (the EagleEyes team) has been onboarded on the Intuition-1 mission by KP Labs. 

# Super-resolution reconstruction

## MuS2
- A Real-World Benchmark for Sentinel-2 Multi-Image Super-Resolution (MuS2) is the dataset, composed of images acquired by Sentinel-2 and WorldView-2 satellites. The S-2 data are organized into tiles, each of which contains a 100 × 100 km MSI, and aggregated into products that are distributed at different processing levels. Here, we exploit Level-2A which includes the bottom of atmosphere reflectance correction. Each tile is composed of 13 spectral bands, however the B10 (cirrus) band is excluded from Level-2A. The blue, green, red, and near infrared (NIR) bands (B02, B03, B04, and B08, respectively) are of 10 m GSD, the vegetation red edge bands (B05, B06, and B07), narrow NIR (B08a), and the short-wave infrared (SWIR) bands (B11 and B12) are of 20 m GSD, while the remaining coastal aerosol (B01), water vapour (B09), and cirrus clouds estimation (B10) bands are of 60 m GSD. Each WV-2 tile contains a panchromatic image of 0.4 m GSD and 8 spectral bands at 1.6 m GSD. These are C–coastal (400–450 nm), B–blue (450–510 nm), G–green (510–580 nm), Y–yellow (585–625 nm), R–red (630–690 nm), RE–red edge (705–745 nm), NIR1 (770–895 nm), and NIR2 (860–1040 nm).
  - metadata: `super-resolution`, <kbd>satellite images</kbd>, `CC-BY`
  - keywords: `image processing`, `machine learning`, `deep learning`, `European Space Agency`, `Sentinel-2`, `WorldView-2`
- DATA FILES: DOI: 10.7910/DVN/1JMRAT 
- CODE: https://codeocean.com/capsule/8131193/tree/v2 
- DATASET PAPER: [Scientific Data](https://doi.org/10.1038/s41597-023-02538-9), [BibTex file](bibtex/mus2.bib)
  - Kowaleczko, P., Tarasiewicz, T., Ziaja, M. et al. A Real-World Benchmark for Sentinel-2 Multi-Image Super-Resolution. Sci Data 10, 644 (2023). https://doi.org/10.1038/s41597-023-02538-9 
    - _Highlights:_ we introduce a new benchmark (named MuS2) for super-resolving multiple Sentinel-2 images, with WorldView-2 imagery used as the high-resolution reference
