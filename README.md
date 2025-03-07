# Implementation-of-DCGAN-on-CelebA-dataset

## Introduction
Deep Convolutional Generative Adversarial Networks (DCGANs) are an improved version of traditional GANs, incorporating convolutional and transposed convolutional layers to enhance stability and performance. Introduced by **Radford et al. (2015)**, DCGANs have been widely used in **image generation tasks**, producing high-quality images by learning features from real datasets.

This project implements a **DCGAN model trained on the CelebA dataset** to generate realistic face images. The experiment follows the architecture and training techniques outlined in the original research paper.

## Dataset Preprocessing
The dataset used is the **CelebA** dataset, which contains over 200,000 images of celebrity faces. Follow these steps to preprocess the dataset:

1. **Download the dataset:**
   - Upload `img_align_celeba.zip` to your Google Drive.
   - Unzip it into the working directory:
    

2. **Apply Transformations:**
   - Resize images to **64x64 pixels**.
   - Apply **center cropping** for better alignment.
   - Convert images to tensors and normalize them to **[-1,1]**.

  

3. **Load Dataset into DataLoader:**
   

## Training the Model
### Steps to Train:
1. **Initialize the DCGAN model** with predefined architectures for the **generator** and **discriminator**.
2. **Define the loss function:** Binary Cross-Entropy (BCE) Loss.
3. **Set up Adam optimizers** for both networks.
4. **Train for multiple epochs**, alternating between training the discriminator and the generator.


## Expected Outputs
- Initially, generated images will appear as **random noise**.
- Over multiple epochs, the generator learns to produce **clearer and more realistic** face images.
- By the end of training, the model should generate **high-quality human faces** resembling those from the CelebA dataset.
- Sample output is available on the repository.

## Conclusion
This project successfully demonstrates the power of **DCGANs** in generating realistic images from the **CelebA dataset**. While the generated images improve over training epochs, further enhancements can be achieved through **hyperparameter tuning, deeper architectures, and longer training cycles**.


