# SpotCheck
## Contents of the Repository
### Section 1: Software and Platform Section
### Section 2: Map of Documentation
### Section 3: Instructions for Reproducing the Results
## Software and Platform

**Software:** Google Colab and Jupyter Notebooks

**Add-on packages:**
- requests
- zipfile
- os
- random
- IPython.display
- Pillow
- numpy
  

**Platform:** Windows and Mac

## Map of the Documentation
```markdown
VaxxVote/
├── data/
│ ├── Coccinella_novemnotata.zip
│ ├── Harmonia_axyridis.zip
│ └── README.md
├── scripts/
│ ├── 1_scraping.ipynb
│ ├── 1_exploratoryplots.ipynb
│ ├── 2_preprocessing.ipynb
│ └── 3_model.ipynb
├── outputs/
│ ├── .png
│ └── .png
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
   pip <insert packages here>
   ```

3. **Run the notebooks in order:**

   **Step 1: Data Cleaning**
   - Open `scripts/1_scraping.ipynb` in Jupyter Notebook or upload to Google Colab
   - Execute all cells in order
   - This will scrape from iNaturalist and create two zip files that are downloaded locally

   **Step 2: Exploratory Analysis**
   - Open `scripts/1_exploratory_plots.ipynb` in Jupyter Notebook or upload to Google Colab
   - Execute all cells in order
   - This will generate descriptive statistics and visualizations in `README.md` in the data folder

   **Step 3: Machine Learning Models**
   - Open `scripts/3_model.ipynb` in Jupyter Notebook or upload to Google Colab
   - Execute all cells in order
   - This will perform the CNN and generate performance visualizations in the `output` folder <and whatever else it does insert here>

**Note:** If using Google Colab, upload the dataset files `Harmonia_axyridis.zip` and `Coccinella_novemnotata.zip` to the `/content/` directory before running the notebooks.
