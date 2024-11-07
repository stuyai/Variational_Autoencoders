# Variational Autoencoders (VAE) on MNIST

By stuyai, taught and made by Otzar Jaffe

This project demonstrates the implementation of a Variational Autoencoder (VAE) using TensorFlow and Keras on the MNIST dataset. The VAE is a generative model that learns to encode input data into a latent space and then decode it back to the original data space.

## Project Structure

- `VAE_MNIST.ipynb`: Jupyter notebook containing the implementation of the VAE model, training process, and visualization of the latent space.
- `requirements.txt`: List of Python packages required to run the project.

## Requirements

To install the required packages, run:
```bash
pip install -r requirements.txt
```

## Usage

1. **Load and preprocess the MNIST dataset**:
    - Normalize the pixel values to the range [0, 1].
    - Reshape the data to include a channel dimension.

2. **Define the VAE model**:
    - **Encoder**: Convolutional layers to encode the input images into a latent space.
    - **Sampling**: Reparameterization trick to sample from the latent space.
    - **Decoder**: Transposed convolutional layers to reconstruct the images from the latent space.

3. **Train the VAE**:
    - Compile the model with an optimizer.
    - Train the model on the MNIST dataset.

4. **Visualize the results**:
    - Plot the 2D manifold of digits in the latent space.
    - Compare original and reconstructed images.

## Example

To run the notebook, execute the following command:
```bash
jupyter notebook VAE_MNIST.ipynb
```

## Results

The notebook includes visualizations of the latent space and reconstructed images, demonstrating the VAE's ability to learn meaningful representations of the MNIST digits.

## License

This project is licensed under the MIT License.
