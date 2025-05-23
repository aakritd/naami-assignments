🦴 CT Bone Segmentation Project
📌 Overview
This project focuses on automatic segmentation and analysis of bones in 3D CT volumes of the knee region. It involves four key subtasks that include image processing-based bone segmentation, mask expansion, randomized contour generation, and anatomical landmark detection. The project works with .nii.gz medical imaging data and aims to support downstream tasks like surgical planning or AI model development.

🚀 Tasks Breakdown
✅ Task 1.1 – Bone Segmentation
Segment the femur and tibia from CT scan slices using thresholding and connected component labeling. The segmentation uses Hounsfield Units to isolate bone structures and identify femur/tibia based on anatomical positioning.

✅ Task 1.2 – Uniform Contour Expansion
Expand the segmentation mask uniformly by 2mm, using a voxel-aware elliptical structuring element to ensure real-world accuracy during morphological dilation.

✅ Task 1.3 – Randomized Contour Adjustment
Generate a randomized expansion of the mask between the original boundary and the 2mm-expanded boundary by scaling the structuring element with a random factor in each slice.

✅ Task 1.4 – Landmark Detection on Tibia
Identify the lowest medial and lateral points on the tibial surface in a selected axial slice. The detected landmarks are visualized for validation and potential biomechanical analysis.

🧰 Tools and Technologies
Language: Python

Platform: Jupyter Notebook

Image Format: .nii.gz (NIfTI format)

Version Control: Git & GitHub

📦 Libraries Used
NumPy, SciPy, SimpleITK, scikit-image, OpenCV, Matplotlib, nibabel

🗃️ Dataset
Input Format: 3D knee CT scans (.nii.gz)

Dimensions: 512 × 512 × N (N = 216)

Example File: 3702_left_knee.nii
