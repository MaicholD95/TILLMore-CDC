# RootTracer Dataset Documentation

## Dataset Overview

The dataset used in the **RootTracer** tool is focused on high-resolution images of plant root systems, specifically barley plants. This dataset provides ground truth annotations for root images, stored in RSML (Root System Markup Language) format, enabling efficient root phenotyping and segmentation for machine learning models.

### Key Features:
- **Plant Type:** Barley (*Hordeum vulgare*)
- **Original Resolution:** 6000x4000 pixels -> cropped and resized
- **Image Format:**  `.jpg`
- **Annotation Format:** RSML
- **Number of Images:** 109 high-resolution root images
- **Annotation Type:** Manual root tracing using RootTracer tool, saved in RSML format or Json format

## Data Structure

### Folder Structure:
- **images/**: Contains the raw high-resolution images of the plant root systems.
- **rsml/**: Contains the RSML files corresponding to each image, with the annotated root systems.
- **json/**: Contains json files with the annotated root points.
  
### File Types:
- **Images**: High-resolution  `.jpg` files of the plant root systems.
- **RSML Files**: XML-based files that represent the root system architectures.

## Annotations

The dataset includes manually annotated root systems, with key points marked along the root structure. The RSML format captures essential features like:
- Root origin
- Root tips
- Intermediate points
- Secondary roots

These annotations serve as the ground truth for training and validating machine learning models for root segmentation.

## Data Collection Process

The barley root images were collected under controlled conditions. The roots were grown in **CD cases** filled with absorbent paper, and images were taken using a **Nikon D5600** camera in a controlled growth chamber. The dataset includes images from different sessions, each exhibiting varying lighting and exposure conditions.

### Dataset Challenges:
- **Variable Backgrounds:** Due to different types of absorbent paper used, background textures vary from smooth to rough, with some showing yellow stains.
- **Lighting Conditions:** Uneven lighting and low contrast in certain sessions.
- **Overlapping Roots:** Each image may contain up to three seeds, and their roots often overlap, making annotation complex.

## Usage

The dataset is designed for use with the **RootTracer** tool for plant phenotyping and root system analysis. It is suitable for:
- Training deep learning models for automated root segmentation.
- Benchmarking automated root phenotyping tools.
- Analyzing root system structures in agricultural research.

## RootTracer Tool
Roottracer is avaiable here [https://github.com/MaicholD95/RootTracer]
## Citation

If you use this dataset in your research, please cite the following publication:

**Maichol Dadi, Alessandra Lumini, Annalisa Franco, Giuseppe Sangiorgi, Silvio Salvi**. RootTracer: An Intuitive Solution for Root Image Annotation. *Computers and Electronics in Agriculture*, 2023.

## Contact

For any questions or issues regarding the dataset, please contact the authors via GitHub issues or email (maichol.dadi2@unibo.it).
