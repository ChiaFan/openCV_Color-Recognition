# openCV_Color-Recognition

Plastic Pellet Contamination Detection

Overview

This project implements a system for detecting contamination in plastic pellet raw materials by analyzing images for color and shape anomalies. The system uses OpenCV, Pillow, and extcolors to process images, filter out specific colors (e.g., white, gray, blue, orange), and identify potential contaminants based on color thresholds and percentage occurrence. It is designed to run on various platforms (PAC, PC, or Colab) and supports both single and multiple image processing for continuous monitoring.

The system logs contaminated images, generates visualizations (e.g., donut plots with color distributions), and manages disk space by removing old files when storage is low. It is suitable for industrial applications requiring automated quality control of plastic pellets.

Features
* Color-Based Contamination Detection: Identifies contaminants by analyzing RGB color values and their percentage occurrence in images, with configurable thresholds.
* Shape Detection (Optional): Detects and counts individual pellets using contour analysis (disabled by default).
* Multi-Platform Support: Configurable for PAC, PC, or Colab environments with appropriate file paths.
* Disk Management: Automatically clears old files when disk usage exceeds 90%.
* Visualization: Generates donut plots showing color distributions alongside the processed image.
* Logging: Records contaminated images in a log file and sets a warning flag for further action.
* Batch Processing: Supports processing multiple images in a directory for continuous monitoring.

Requirements
* Python 3.8+
* OpenCV (cv2)
* NumPy
* Pandas
* Matplotlib
* Pillow (PIL)
* extcolors
* colormap
* shutil
