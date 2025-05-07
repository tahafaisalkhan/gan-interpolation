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

## 📊 Results

- Generator loss converged to a stable minimum after ~50 epochs.
- The best MNIST generator produces clear digit-like outputs.
- Interpolation between latent vectors shows smooth transitions between digits and faces.
- Vector arithmetic in the latent space reflects meaningful compositional image edits (e.g., smile + glasses).

## 🖼️ Visuals

| Training Losses | Best MNIST Sample | MNIST Interpolation |
|-----------------|-------------------|----------------------|
|![asdasdasdasd](https://github.com/user-attachments/assets/c146b096-6f81-49ac-9753-8a1dd7cea106)
 |  ![asdasdasdasda](https://github.com/user-attachments/assets/e44c0c72-e618-400e-b1a6-a2e8fcc27494)
| ![asdasdasda](https://github.com/user-attachments/assets/f34e38b6-b2c9-43ad-963c-de3bf33567e7)|

| CelebA Interpolation | Arithmetic A + B | Arithmetic E - F + G |
|----------------------|------------------|------------------------|
| ![asdsad](https://github.com/user-attachments/assets/b20ea0de-87be-41e5-a3a9-8c0480d9978c)
 | ![output](https://github.com/user-attachments/assets/b1c903da-52d7-49de-8946-f1d28f8d8404)
 | ![asd](https://github.com/user-attachments/assets/d78de854-fb01-41dc-9a7a-14727392d574)|

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
