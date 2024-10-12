# Developing a Predictive Model in GST

The purpose of this Hackathon is to engage Indian students, researchers, and innovators in developing advanced, data-driven AI and ML solutions based on given data set. Participants will have access to a comprehensive data set containing approximately 900,000 records, each with around 21 attributes and target variables. This data is anonymized, meticulously labeled, and includes training, testing, and a non-validated subset reserved specifically for final evaluations by the GSTN.

Participants are encouraged to use this dataset to design and implement innovative artificial intelligence (AI) and machine learning (ML) algorithms to tackle the stated challenge.

Additionally, this initiative aims to foster collaboration between academia and industry professionals, driving the development of effective and insightful solutions that strengthen the GST analytics framework.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Installation

To run the entire code, you need two versions of Python. One must be higher than version 3.10 to calculate some attributes, and Python version 3.10 to give conclusions using PyCaret. A devcontainer is provided for Python version 3.10.

### Python Installation

Ensure you have both Python versions installed on your system.

#### Install Python 3.10

```bash
# For Ubuntu
sudo apt update
sudo apt install python3.10

# For Windows
# Download the installer from https://www.python.org/downloads/release/python-3100/
# Run the installer and follow the instructions
```

#### Install Python >3.10

```bash
# For Ubuntu
sudo apt update
sudo apt install python3.11

# For Windows
# Download the installer from https://www.python.org/downloads/release/python-3110/
# Run the installer and follow the instructions
```

### Using Devcontainer for Python 3.10

A devcontainer is provided for Python version 3.10. To use it, follow these steps:

1. Ensure you have Docker installed on your system.
2. Open your project in Visual Studio Code.
3. Add a `.devcontainer` folder in the root of your project with the following files:

**`devcontainer.json`**
```json
{
    "name": "Python 3.10",
    "image": "python:3.10",
    "postCreateCommand": "pip install -r requirements.txt",
    "extensions": [
        "ms-python.python"
    ]
}
```

**`Dockerfile`**
```Dockerfile
FROM python:3.10

# Set the working directory
WORKDIR /workspace

# Copy the current directory contents into the container
COPY . /workspace

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt
```

4. Reopen the project in the container by clicking on the green button in the bottom-left corner of VS Code and selecting "Reopen in Container".

This setup ensures that you have a consistent development environment with Python 3.10.


## Usage

Provide instructions and examples for using your project.


It can simply give the conclusion by seeing the outputs attached with code.

## Contributing

@BLANK0104

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
