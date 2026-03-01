# Cinematic Color Palette Generator

An interactive Python tool built in Google Colab that uses **K-Means Clustering** (Unsupervised Machine Learning) to extract dominant color palettes from movie screenshots or photography.

## Overview
This project treats every pixel in an image as a data point in a 3D RGB space. By applying the K-Means algorithm, the tool identifies the $K$ most representative colors, providing designers and photographers with a "cinematic" color story for any frame.

## Features
* **Batch Image Handling:** Upload multiple images at once and choose which one to analyze via a user-input prompt.
* **Machine Learning Integration:** Utilizes `scikit-learn`'s K-Means to cluster color data.
* **Big Data Optimization:** Implements image resizing to maintain high performance without losing color accuracy.
* **Designer-Ready Output:** Displays the original image alongside a clean palette strip with generated **Hex codes**.

## Tech Stack
* **Language:** Python
* **IDE:** Google Colab
* **Libraries:** `OpenCV`, `NumPy`, `Matplotlib`, `scikit-learn`

## How to Use
1. Open the `.ipynb` file in Google Colab.
2. Run the first block to import libraries.
3. Upload your images (e.g., `Kenjaku.jpg`, `Gojo.png`) when prompted.
4. Type the filename of the specific image you want to analyze.
5. The tool will output the visual palette and the corresponding Hex codes.

## Future Improvements
* Add an "Elbow Method" graph to programmatically determine the optimal number of colors.
* Implement an export feature to save the palette as a `.png` or `.json` file.