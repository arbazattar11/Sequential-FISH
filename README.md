### Sequential FISH (Fluorescence In Situ Hybridization) Data Analysis Pipeline

Sequential FISH is a powerful technique used to visualize and quantify multiple nucleic acid sequences in single cells. This pipeline will guide you through the analysis of Sequential FISH data, including image processing, spot detection, decoding, registration, and visualization.
# Sequential FISH Data Analysis Pipeline

This pipeline provides a step-by-step workflow for processing and analyzing Sequential Fluorescence In Situ Hybridization (FISH) data. It includes image processing, spot detection, decoding, registration, and visualization.

## Prerequisites

Ensure the following tools and libraries are installed and accessible:

- Python 3
- NumPy
- SciPy
- scikit-image
- OpenCV
- pandas
- matplotlib
- seaborn
- tifffile
- napari

You also need image files from Sequential FISH experiments.

## Directory Structure

- `raw_images`: Directory containing raw image files.
- `processed_images`: Directory for storing processed images.
- `results`: Directory for storing analysis results.
- `visualization`: Directory for storing visualization outputs.

## Usage

1. **Set Up the Directories**:
    Ensure the necessary directories exist or create them:

    ```bash
    mkdir -p raw_images processed_images results visualization
    ```

2. **Prepare Image Data**:
    Ensure the raw image files are available in the `raw_images` directory.

3. **Run the Script**:
    Save the pipeline script as `sequential_fish_pipeline.py` and run it using Python:

    ```bash
    python sequential_fish_pipeline.py
    ```

## Script Breakdown

### Step 1: Image Preprocessing

Perform background subtraction, noise reduction, and other preprocessing steps on raw images.

### Step 2: Spot Detection

Identify and localize fluorescent spots in each image.

### Step 3: Decoding

Decode the sequential FISH barcodes to identify specific nucleic acid sequences.

### Step 4: Registration

Align and register images from different cycles to ensure accurate decoding.

### Step 5: Visualization

Visualize the detected spots and decoded sequences.

## Notes

- Modify the paths and parameters in the script as needed.
- Ensure all input files (e.g., image files) are correctly specified.
- The pipeline assumes single-channel Sequential FISH data; for multi-channel data, adjustments might be needed.

## References

- [NumPy](https://numpy.org/)
- [SciPy](https://www.scipy.org/)
- [scikit-image](https://scikit-image.org/)
- [OpenCV](https://opencv.org/)
- [pandas](https://pandas.pydata.org/)
- [matplotlib](https://matplotlib.org/)
- [seaborn](https://seaborn.pydata.org/)
- [tifffile](https://pypi.org/project/tifffile/)
- [napari](https://napari.org/)

## License

This project is licensed under the MIT License - see the LICENSE file for details.
