# Development and assessment of an AI-based tool for scoring lesion severity in generalized pustular psoriasis clinical images (AGPPGA)

## Project Description

This repository serves as the central data hub for the research article: **"Development and assessment of an AI-based tool for scoring lesion severity in generalized pustular psoriasis clinical images"**.

The goal of this project was to develop **AGPPGA** (Automatic Generalized Pustular Psoriasis Physician Global Assessment), an artificial intelligence framework designed to assess the severity of Generalized Pustular Psoriasis (GPP) lesions from clinical images. By automating the grading of key visual signs—pustules, erythema, and scaling—this tool aims to reduce inter-rater variability and assist clinicians in making more objective severity assessments.

This repository provides access to the Non-Specific Lesion (NSL) dataset, a curated index of public image sources, and detailed instructions for requesting access to the clinical trial data.

## Dataset Subsets

The study utilized three distinct image subsets to train and validate the AI model. Below is a description of each, along with instructions on how to access the data.

### 1. Non-Specific Lesion (NSL) Dataset

**Description:** This dataset contains images of healthy skin or non-specific lesions that do not exhibit GPP symptoms. It was used to "anchor" the model's baseline for clear skin (GPPGA score = 0), improving its ability to distinguish low-severity lesions from normal skin.

The NSL dataset consists of two subsets from which extra image crops are generated:

1. **Internet-Sourced Subset:** Images of healthy skin compiled from open internet sources. Due to licensing restrictions, we do not host these image files directly. Instead, a list of their original source URLs is provided in the file: `/data/NSL/internet_images_urls.txt`.

2. **Consented Subset:** Non-identifiable images of healthy skin taken specifically for this study from volunteers who provided formal written informed consent. The full image files are hosted directly in this repository in the `/data/NSL/consented_images/` folder.

### 2. V1 Dataset (Public & Clinical Trial Mix)

**Description:** A collection of images of GPP lesions.

**Composition:** images sourced from public dermatology atlases and a clinical trial.

**Image Type:** These images typically capture only the specific lesion area, excluding the rest of the patient's body.

**Access:**

1. **Public Images:** Sourced from [Dermatology Atlas](https://www.atlasdermatologico.com.br/), [Danderm](https://danderm-pdv.is.kkh.dk/), [DermNet NZ](https://dermnetnz.org/), [DermIS](https://www.dermis.net/dermisroot/en/home/index.html) (https://doi.org/10.1111/j.1346-8138.1998.tb02505.x).

2. **Private Images:** Sourced from the `EFFISAYIL® 1` clinical trail. See the *Private Data Access* section below.

### 3. V2 Dataset

**Description:** A large dataset of high-resolution images from 46 patients.

**Source:** Data from the `EFFISAYIL® 2` clinical trial.

**Image Type:** High-resolution photographs capturing larger body areas (e.g., full back, lower limbs), taken in a standardized clinical setting.

**Access:** See the *Private Data Access* section below.


## Access to the EFFISAYIL® 1 and EFFISAYIL® 2 data

1. **EFFISAYIL® 1 (NCT03782792):** *Trial of Spesolimab for Generalized Pustular Psoriasis*. **DOI:** [10.1056/NEJMoa2111563](https://doi.org/10.1056/NEJMoa2111563)

2. **EFFISAYIL® 2 (NCT04399837):** *Efficacy and safety of subcutaneous spesolimab for the prevention of generalised pustular psoriasis flares (Effisayil 2): an international, multicentre, randomised, placebo-controlled trial*. **DOI:** [10.1016/S0140-6736(23)01378-8](https://doi.org/10.1016/S0140-6736(23)01378-8)

**How to Request Access:**

Qualified scientific and medical researchers may request access to these datasets (including participant-level data). Requests must be made through the **[Vivli.org](https://vivli.org/)** data-sharing platform or by contacting the corresponding authors of the primary publications listed above. Find more details in their respective original publications.

## Ethics, Consent, and Usage

**NSL Dataset (Consented):** Images in the /data/NSL/consented_images/ folder were collected with formal written informed consent from all participants. These images are strictly non-identifiable and were obtained specifically for research purposes.

**NSL Dataset (Internet):** Images referenced in /data/NSL/internet_images_urls.txt were sourced from open internet repositories and used in accordance with their respective source policies.

**Atlas images:** All images sourced from public dermatology atlases were used in strict accordance with their respective source policies and ethical guidelines.

**Clinical trial images:** Images from the EFFISAYIL® 1 and 2 trials were obtained and used in accordance with the ethical approvals, informed consent protocols, and data sharing specifications detailed in their respective primary publications.

**Software Code:** The AGPPGA software code is proprietary to **Legit.Health** and is not available for public distribution.

**Usage Note:** The data provided in this repository is for research and validation purposes only. Any use of the images must comply with the original copyright holders' terms.


## License
The datasets, images, and documentation in this repository are licensed under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license.
**You are free to:**
* **Share** — copy and redistribute the material in any medium or format.
* **Adapt** — remix, transform, and build upon the material for any purpose, even commercially.


**Under the following terms:**
* **Attribution** — You must give appropriate credit, provide a link to the license, and indicate if changes were made.


**Note on Software:**
The **AGPPGA software code** and model weights are **proprietary intellectual property of Legit.Health** and are **NOT** included in this license. This repository provides only the dataset information and documentation necessary for methodological replication.
