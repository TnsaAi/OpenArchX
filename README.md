# OpenArchX

OpenArchX is a deep learning framework designed for efficient model training and inference, with support for CUDA operations using CuPy. This framework is built to be independent of PyTorch while providing similar functionalities.

## Features

- **CUDA Support**: Leverage GPU acceleration for faster computations.
- **Custom Tensor Implementation**: A flexible tensor class that supports both CPU and GPU operations.
- **Modular Design**: Easily extendable architecture for adding new layers, optimizers, and utilities.

## Requirements

- Python 3.8 or higher
- NumPy
- CuPy (with CUDA support)
- Other dependencies as specified in `requirements.txt`

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/OpenArchX.git
   cd OpenArchX
   ```

2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Install CuPy with the appropriate CUDA version:
   ```bash
   pip install cupy-cuda112  # Replace with your CUDA version
   ```

## Usage

To train the MNIST model using OpenArchX, run the following command:

```bash
python examples/mnist_cnn.py --cuda  # Use --cpu to run on CPU
```

## Testing

You can run the CUDA tests to ensure everything is set up correctly:

```bash
python -m openarchx.cuda.test_cuda
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [CuPy](https://cupy.dev/) for GPU support.
- [NumPy](https://numpy.org/) for numerical operations.
