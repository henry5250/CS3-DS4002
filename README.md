# SpotCheck
## Contents of the Repository
### Section 1: Software and Platform Section
### Section 2: Map of Documentation
### Section 3: Instructions for Reproducing the Results
## Software and Platform

**Software:** Google Colab

**Add-on packages:**
- requests
- zipfile
- pandas
- os
- random
- time
- IPython.display
- Pillow
- numpy
- tensorflow
- matplotlib.pyplot

**Platform:** Windows and Mac

## Map of the Documentation
```markdown
VaxxVote/
├── data/
│ ├── final_datasets/
│ │ ├── final_Coccinella_novemnotata.zip
│ │ └── final_Harmonia_axyridis.zip
│ ├── original_datasets/
│ │ ├── Coccinella_novemnotata.zip
│ │ └── Harmonia_axyridis.zip
│ └── README.md
├── scripts/
│ ├── 1_scraping.ipynb
│ ├── 2_exploratoryplots.ipynb
│ ├── 3_preprocessing.ipynb
│ ├── 4_model.ipynb
├── outputs/
│ ├── exploratory_plots/
│ │ ├── f_pixel intensity histogram for Coccinella_novemnotata (RGB channels).png
│ │ ├── f_pixel intensity histogram for Coccinella_novemnotata (RGB channels).png
├── visualizations/
│ │ ├── f_test accuracy for different hyperparams.png
│ │ ├── f_test loss for different hyperparams.png
│ │ └── .png
├── LICENSE
└── README.md
```

## Instructions for Reproducing the Results

1. **Clone the repository:**
   ```bash
   git clone https://github.com/henry5250/SpotCheck.git
   cd SpotCheck
   ```

2. **Install required packages:**
   ```bash
   pip zipfile, pandas, os, random, time, IPython.display, Pillow, numpy, tensorflow, matplotlib.pyplot
   ```

3. **Run the notebooks in order:**

   **Step 1: Data Cleaning**
   - Open `scripts/1_scraping.ipynb` in Jupyter Notebook or upload to Google Colab
   - Execute all cells in order
   - This will scrape from iNaturalist and create two zip files that are downloaded locally

   **Step 2: Exploratory Analysis**
   - Open `scripts/2_exploratory_plots.ipynb` in Jupyter Notebook or upload to Google Colab
   - Execute all cells in order
   - This will generate descriptive statistics and visualizations in `README.md` in the data folder
   
   **Step 3: Preprocessing**
   - Open `scripts/3_preprocessing.ipynb` in Jupyter Notebook or upload to Google Colab
   - Execute all cells in order
   - This will process the zipfiles that were scraped and make it possible to run the model through testing hyperparameters.

   **Step 4: Machine Learning Models**
   - Open `scripts/4_model.ipynb` in Jupyter Notebook or upload to Google Colab
   - Execute all cells in order
   - This will perform the tensorflow and generate performance visualizations in the `output` folder.

**Note:** If using Google Colab, upload the dataset files `Harmonia_axyridis.zip` and `Coccinella_novemnotata.zip` to the `/content/` directory before running the notebooks. Use the TPU runtime to speed up the processing.
