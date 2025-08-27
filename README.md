# LSENS-Lab-Immersion
Data management internship at the EPFL Brain Institute’s LSENS lab, working with published and unpublished neurophysiological datasets. This repository summarizes my work on converting data to the NWB format and developing small analysis pipelines from the converted datasets. Voici une version améliorée et traduite en anglais :

> For more details, you can also refer to the PDF in this repository, which is my internship report and contains valuable technical information about the different pipelines.


## 📁 Related Repositories
### 1. NWB Conversion Pipeline (Oryshchuk et al., 2024)


This repository converts behavioral and electrophysiological data from **Oryshchuk et al., 2024 (Cell Reports)** into the standardized **Neurodata Without Borders (NWB)** format.  
The study investigates how sensory, motor, and decision-related information is distributed and encoded in the mouse neocortex during goal-directed behavior.  

For detailed usage and dataset-specific notes, see the full README of this repository.

Reference: 👉 [DOI](https://doi.org/10.1016/j.celrep.2023.113618)

Repository: 🔗 [Github](https://github.com/loris-fab/NWB_converter_AN.git)


#### 1.1 📊 Template Matching GUI (Oryshchuk et al., 2024)

Custom analysis interface tailored for **NWB-formatted datasets** from *Oryshchuk et al., 2024, Cell Reports*.  
Provides advanced PSTH exploration, trial-based filtering, and decoder tuning to analyze the study’s behavioral and electrophysiological recordings.

Repository: 🔗 [Github](https://github.com/loris-fab/NWB_Whisker-Stimulus-Decoding-main.git)

---
### 2. NWB Conversion Pipeline (Pierre Le Merre et al., 2018, Cell Reports)

Converts behavioral and electrophysiological data from **Pierre Le Merre et al., 2018 (Cell Reports)** into the **Neurodata Without Borders (NWB)** format.  
The study examines how distributed brain networks encode and integrate sensory, motor, and cognitive signals during goal-directed behavior in mice.

For detailed usage and dataset-specific notes, see the full README of this repository.

Reference: 👉 [DOI](https://pmc.ncbi.nlm.nih.gov/articles/PMC5766832/)

Repository: 🔗 [Github](https://github.com/loris-fab/NWB_Converter_LeMerre.git)

---

### 3. NWB Conversion Pipeline (unpublished, 2025)

Converts **single-neuron membrane potential recordings** from the medial prefrontal cortex (mPFC) of awake behaving mice into the **Neurodata Without Borders (NWB)** format.

The dataset includes two experimental conditions:

Since there is no published article yet, the dataset contains single-neuron membrane potential recordings from the medial prefrontal cortex of awake mice: Whisker rewarded (WR+) mice received water if they licked within 1 s after a whisker stimulus (go trials), but not in no-go trials; No-Task mice were head-fixed and received random whisker stimuli without a task. Recordings were obtained using whole-cell patch-clamp.

For detailed usage and dataset-specific notes, see the full README of this repository.

Repository: 🔗 [Github](https://github.com/loris-fab/NWB_converter_PB.git)


## ⚙️ Environment setup

### Install Anaconda

1. Download the installer from [Anaconda official website](https://www.anaconda.com/download).  
2. Verify installation:  
   ```bash
   conda --version
   ```
### Create and activate an environment:

Download the **requirements.txt** file from the current repository.  
Then, open a terminal in the same directory and run the following command:


```bash
conda create -n nwb_env python=3.9
conda activate nwb_env
python -m pip install --upgrade pip wheel setuptools && pip install -r requirements.txt
```
