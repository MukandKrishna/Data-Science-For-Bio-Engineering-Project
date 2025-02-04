# Image-Based Bioengineering Data Analysis and Query Tool

## Overview
This project automates the analysis of bioengineering experiment images containing cell groups. It extracts key attributes, organizes them into structured data, and enables efficient querying and visualization.

## Features
- **Automated Image Processing**: Identifies and segments individual cells.
- **Feature Extraction**: Measures cell size, shape, position, and density.
- **Structured Data Output**: Converts image data into an Excel table.
- **Query and Visualization**: Enables user-friendly data querying and visualization.

## Folder Structure
```
📂 Data-Science-For-Bio-Engineering-Project
├── 📂 cleared/             # Folder for clear images
├── 📂 shaded/             # Folder for shady images
├── 📂 Projecr description.docx/             # Processed results and visualizations
├── 📜 Project_Code.ipynb  # Jupyter Notebook for image analysis
├── 📜 images_analysis.xlsx # Extracted data in tabular format
├── 📜 README.md           # Project documentation (this file)
```

## Methodology
### Step 1: Image Processing
- Loaded the dataset of images containing bioengineered cells.
- Applied **grayscale conversion** and **contrast enhancement** to improve segmentation.
- Used **Watershed Segmentation** to detect and isolate individual cells.

### Step 2: Feature Extraction
- Extracted key attributes for each cell:
  - **Size**: Measured pixel area.
  - **Shape**: Calculated circularity and aspect ratio.
  - **Position**: Identified centroid coordinates.
  - **Density**: Estimated based on cell count per image.
- Summarized results at both cell level and image level.

### Step 3: Data Storage and Output
- Organized extracted data into a structured **Excel file (`images_analysis.xlsx`)**.
- Each row represents a detected cell with its respective attributes.
- Additional sheet contains summary statistics for each image.

### Step 4: Visualization & Querying
- Generated **histograms and scatter plots** to analyze feature distributions.
- Enabled **interactive querying** to filter images based on cell characteristics.

## Results
- Successfully processed **all input images** and extracted meaningful features.
- Average cell size distribution showed **X-Y variation**.
- High-density images exhibited **clustering effects**, influencing segmentation.
- Querying tool allowed retrieval of **specific cell populations** efficiently.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Image_Analysis_Project.git
   ```
2. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Project_Code.ipynb
   ```

## Usage
- **Run the notebook** to process images and extract features.
- **Check `images_analysis.xlsx`** for tabular results.
- **Modify the code** to customize feature extraction.

## Contributors
This project was developed collaboratively by:
- **Mukand Krishna** - Lead Developer
- **Noreen Fatima**
- **Muhammad Zain Ul Aabedin**
- **Jawad Ahmed**
- **Yasmin Al-Omary**
- 
## Contributing
Feel free to fork this repository and submit pull requests for improvements.

## License
This project is open-source under the MIT License.
