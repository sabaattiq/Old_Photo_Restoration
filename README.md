# Old_Photo_Restoration
This project uses deep learning to restore old photos through a step-by-step process of super-resolution, face enhancement, and colorization. It improves image quality and adds color with minimal user input, making it ideal for use in archives, museums, and family albums.
Introduction

Old photographs are prone to quality degradation such as blurring, scratches, and loss of color over time. Manual restoration is a labor-intensive and skill-dependent task. With the advent of modern machine learning methods, automated photo restoration can now be performed with impressive accuracy. This project aims to automate the restoration of old and damaged photographs by using a stepwise AI pipeline consisting of image enhancement, face restoration, and colorization modules.
Problem Statement

Manual restoration of historical and family photos is time-consuming, costly, and requires professional expertise. The core problems include low resolution, facial detail loss, and absence of color. This project addresses these challenges by proposing an AI-based solution that is both efficient and accessible.

Objectives

	Develop a user-friendly AI pipeline for old photo restoration
	Integrate tools for super-resolution
	Apply facial enhancement techniques
	Implement colorization methods
	Design a minimal interface within Google Colab using executable notebook cells for end-to-end pipeline demonstration
Technologies Used

	Python
	Google Colab (Interface)
	Real-ESRGAN (Super Resolution)
	GFPGAN (Face Restoration)
	DDColor (Colorization)
	OpenCV, NumPy, Matplotlib (Image Processing & Visualization)
System Architecture

The restoration system follows a modular architecture:
1.	Image Upload: Users upload black-and-white or degraded images.
2.	Super-Resolution: Enhances the resolution of the uploaded images.
3.	Face Enhancement: Restores facial details in portrait images.
4.	Colorization: Adds realistic color to grayscale images.
5.	Output Display: Results are shown side-by-side for comparison.
The interface handles user input and output display seamlessly without external libraries like Gradio, relying on the native capabilities of Google Colab notebooks.
Implementation Details

The project notebook executes the following key steps:
	Installation of dependencies and cloning of relevant repositories
	Downloading pre-trained weights for each processing stage
	Image upload interface via Google Colab widgets
	Function to run each pipeline step: 
Super-resolution → Facial restoration → Colorization
	Output visual comparison using Matplotlib
 
Each component is encapsulated to ensure modularity and clarity. The notebook is hosted and executed on Google Colab.
The output images demonstrate the effectiveness of the pipeline. Users can clearly see the transition from grayscale, blurry input to colorized, facially restored output. Each stage adds distinct visual improvements, culminating in high-quality restored photographs suitable for archival purposes.
Results and Evaluation

	High-quality image enhancement observed
	Clear facial restoration in images containing faces
	Colorization results appear realistic, although some inconsistencies may occur in background areas
	User interface ensures accessibility and ease of use directly within Colab
	Users can visualize all transformation stages in one interactive environment
Challenges Faced

	Handling large model sizes within the Colab environment
	Compatibility issues between different software dependencies
	Ensuring consistent output across a variety of input images
	Minor artifacts in facial restoration when input image is heavily damaged
	Color inaccuracies in highly deteriorated or low-contrast images
Conclusion

The project successfully demonstrates an AI-based pipeline for old photo restoration, combining multiple deep learning techniques into a single workflow. The results show significant improvement in image resolution, clarity, and realism. The interface allows users to engage with the system easily, making it suitable for public or institutional use.
Future Work

1.	Integrate damage detection and scratch removal; add support for batch processing
2.	Improve facial recognition and background harmony in colorization
3.	Deploy as a standalone desktop or mobile application
4.	Collect region-specific datasets for culturally accurate photo restoration
References
1. Real-ESRGAN: https://github.com/xinntao/Real-ESRGAN
2. GFPGAN: https://github.com/TencentARC/GFPGAN

