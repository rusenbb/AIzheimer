# AIZHEIMER: How was I Drawing?

## Overview

**AIZHEIMER: How was I Drawing?** is a project aimed at exploring the concept of "unlearning" in AI models, specifically focusing on the Stable Diffusion model. The project demonstrates how to selectively forget certain concepts from a pre-trained model using custom attention mechanisms and loss functions.

The offficial introduction video (it is a parody video 😂):

[AIZHEIMER: How was I Drawing? <svg viewBox="0 0 97 20" xmlns="http://www.w3.org/2000/svg" width="48.5" height="10">
<path d="M27.9704 3.12324C27.6411 1.89323 26.6745 0.926623 25.4445 0.597366C23.2173 2.24288e-07 14.2827 0 14.2827 0C14.2827 0 5.34807 2.24288e-07 3.12088 0.597366C1.89323 0.926623 0.924271 1.89323 0.595014 3.12324C-2.8036e-07 5.35042 0 10 0 10C0 10 -1.57002e-06 14.6496 0.597364 16.8768C0.926621 18.1068 1.89323 19.0734 3.12324 19.4026C5.35042 20 14.285 20 14.285 20C14.285 20 23.2197 20 25.4468 19.4026C26.6769 19.0734 27.6435 18.1068 27.9727 16.8768C28.5701 14.6496 28.5701 10 28.5701 10C28.5701 10 28.5677 5.35042 27.9704 3.12324Z" fill="#FF0000"></path>
<path d="M11.4275 14.2854L18.8475 10.0004L11.4275 5.71533V14.2854Z" fill="white"></path>
</svg>](https://www.youtube.com/watch?v=kRVybM5KQ3g)

## Table of Contents

- [Overview](#overview)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributors](#contributors)
- [License](#license)

## Installation

To set up the project, follow these steps:

1. **Clone the repository:**

   ```bash
   git clone git@github.com:rusenbb/AIzheimer.git
   cd aizheimer
   ```

2. **Install the required packages:**
   You can run the first cell in the Jupyter notebook to install the necessary packages or use the following command:

   ```bash
   pip install diffusers transformers accelerate torchmetrics[image] torch-fidelity
   ```

3. **Download the necessary models:**
   Ensure you have the required models from Hugging Face or other sources as specified in the notebook.
   The models should be automatically downloaded if not locally available. So it should not be a problem.

## Usage

1. **Run the Jupyter Notebook:**
   Open the `aizheimer_main.ipynb` notebook in Jupyter and follow the instructions to execute the cells. This notebook contains the entire workflow for setting up the environment, preparing the data, training the model, and testing the results.

2. **Configuration:**
   You can configure various parameters such as `model_save_path`, `concept_to_forget`, `num_image_generate`, `num_epochs`, `batch_size`, `learning_rate`, and `weight_decay` in the notebook.

3. **Training:**
   The training process involves using custom attention mechanisms and loss functions to selectively forget the specified concept from the model.

4. **Inference:**
   After training, you can test the model by generating images and observing the results to ensure the specified concept has been forgotten.

## Project Structure

```
AIZHEIMER/
├── README.md
├── aizheimer_main.ipynb
└── generated_images/
```

- **README.md:** This file.
- **aizheimer_main.ipynb:** Jupyter notebook containing the main code for the project.
- **generated_images/:** Directory for storing generated images or training images.

IMPORTANT:

```
If you decided to not use model generated the images,
you should have training images in the generated_images folder.
```

## Contributors

- **Muhammed Ruşen Birben**
- **Göktürk Batın Dervişoğlu**
- **Abdulkadir Külçe**

We would like to thank our advisor **Behçet Uğur Töreyin** for his guidance and support throughout the project.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
