# Real Estate Image Classification

A pet project aimed at developing a neural network capable of determining specific parameters of apartments from advertisement photos, such as the presence of an air conditioner, washing machine, oven, etc. The model also classifies the quality of the renovation, distinguishing between "grandma's repair" and modern repair.

The project includes a web interface deployed on a server, allowing users to input a link to an apartment advertisement and receive results indicating the quality of the repair and the presence of specific equipment.

## Table of Contents

- [Features](#features)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Image Parsing**: Extract photos from apartment advertisements.
- **Equipment Detection**: Identify the presence of appliances like air conditioners, washing machines, ovens, etc.
- **Renovation Quality Classification**: Classify apartments into "grandma's repair" or modern repair based on images.
- **Web Interface**: Users can input advertisement links and receive classification results.
- **Open Source**: Code is available on GitHub for collaboration and contributions.

## Project Structure

```
real_estate_image_classification/
├── data/               # Datasets and processed data
├── src/                # Source code for the project
├── tests/              # Unit and integration tests
├── venv/               # Virtual environment for Python packages
├── README.md           # Project documentation
└── requirements.txt    # List of project dependencies
```

- **data**: Contains datasets and any preprocessed data required for training and testing the model.
- **src**: Includes all the source code, such as data parsers, model training scripts, and the web application code.
- **tests**: Holds all the tests to ensure code reliability and correctness.
- **venv**: A virtual environment for managing Python dependencies specific to this project.
- **README.md**: Provides an overview and documentation of the project.
- **requirements.txt**: Lists all Python packages and their versions needed to run the project.

## Installation

### Prerequisites

- **Python 3.8 or higher**
- **Git**
- **Virtual Environment Tool**: `venv` or `virtualenv`

### Steps

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/real_estate_image_classification.git
   cd real_estate_image_classification
   ```

2. **Create a Virtual Environment**

   ```bash
   python -m venv venv
   ```

3. **Activate the Virtual Environment**

   - On Windows:

     ```bash
     venv\Scripts\activate
     ```

   - On Unix or MacOS:

     ```bash
     source venv/bin/activate
     ```

4. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

## Usage

### Data Parsing

Before training the model, you need to parse images from apartment advertisements.

```bash
python src/data_parser.py
```

### Model Training

Train the neural network using the parsed data.

```bash
python src/train_model.py
```

### Running the Web Interface

Start the web server to use the application.

```bash
python src/app.py
```

Open your web browser and navigate to `http://localhost:5000` to use the application.

## Contributing

Contributions are welcome! Please follow these steps:

1. **Fork the Repository**

2. **Create a Feature Branch**

   ```bash
   git checkout -b feature/YourFeature
   ```

3. **Commit Your Changes**

   ```bash
   git commit -m "Add your message"
   ```

4. **Push to the Branch**

   ```bash
   git push origin feature/YourFeature
   ```

5. **Open a Pull Request**

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.