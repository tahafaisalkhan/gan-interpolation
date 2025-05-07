# GANs and Latent Space Interpolation 🧠✨

This project demonstrates the use of Generative Adversarial Networks (GANs) for generating synthetic images, exploring the latent space of generative models, and performing meaningful vector arithmetic on image representations. It also includes training a GAN on the MNIST dataset and working with a pre-trained GAN on the CelebA dataset.

## 🔧 Project Structure

- **MNIST GAN Training**
  - Builds a simple fully connected generator and convolutional discriminator.
  - Trains on the MNIST dataset.
  - Tracks generator and discriminator losses.
  - Saves the best performing models.

- **Image Generation**
  - Visualizes outputs from the best trained generator.

- **Latent Space Interpolation**
  - Interpolates between two noise vectors to see how the generator transitions between digit styles.
  - Repeats the process using a pre-trained GAN on the CelebA face dataset.

- **Latent Vector Arithmetic**
  - Demonstrates how adding and subtracting vectors in the latent space can manipulate image features (e.g., smiling + glasses).

## 📁 Files

- `generator.pth` and `discriminator.pth`: Saved models for MNIST.
- `dcgan.py`: Class to interface with the pre-trained CelebA GAN.
- `generator.pt`: Pre-trained CelebA generator weights.
- Multiple `.png` files: Generated visual outputs including:
  - Training losses
  - Best generator sample
  - Latent space interpolations (MNIST and CelebA)
  - Vector arithmetic examples

## 📊 Results

- Generator loss converged to a stable minimum after ~50 epochs.
- The best MNIST generator produces clear digit-like outputs.
- Interpolation between latent vectors shows smooth transitions between digits and faces.
- Vector arithmetic in the latent space reflects meaningful compositional image edits (e.g., smile + glasses).

## 🖼️ Visuals

| Training Losses | Best MNIST Sample | MNIST Interpolation |
|-----------------|-------------------|----------------------|
| ![Training Losses](./6926ac6b-f7e9-4400-9180-83507608b459.png) | ![Best MNIST Sample](./2f64cdc2-24f4-44f2-bca1-ceb0615dcc23.png) | ![MNIST Interpolation](./5109b5d2-58ef-4d29-aa3c-bed93fa77af1.png) |

| CelebA Interpolation | Arithmetic A + B | Arithmetic E - F + G |
|----------------------|------------------|------------------------|
| ![CelebA Interpolation](./fc6a6a80-ef89-44ff-a37f-4616712f0d5d.png) | ![A + B](./32e57a79-e4a1-4693-9c48-627e274027c5.png) | ![E - F + G](./9e7ae81d-6a86-45eb-bf08-86806183363d.png) |

## 🧠 Key Concepts

- **GANs (Generative Adversarial Networks)**: A generator learns to produce realistic images while a discriminator tries to distinguish real from fake data.
- **Latent Space**: The space of input noise vectors for the generator; structured enough to allow interpolation and arithmetic.
- **Mode Collapse**: A common GAN issue where the generator produces limited variety.
- **Vector Arithmetic**: Enables manipulation of image features (e.g., adding smile, removing glasses).

## ✅ Requirements

- Python 3.7+
- PyTorch
- torchvision
- matplotlib
- numpy
