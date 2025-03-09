# ThokNaath: Nuer Language TTS and STT

ThokNaath is an open-source project aimed at developing **Text-to-Speech (TTS)** and **Speech-to-Text (STT)** systems for the Nuer language. The goal is to empower communication, education, and cultural preservation by making Nuer language technology accessible to everyone.

## Table of Contents
1. [Project Structure](#project-structure)
2. [Getting Started](#getting-started)
   - [Prerequisites](#prerequisites)
   - [Installation](#installation)
3. [Usage](#usage)
   - [TTS System](#tts-system)
   - [STT System](#stt-system)
4. [Development](#development)
   - [Data Collection](#data-collection)
   - [Model Training](#model-training)
   - [Testing](#testing)
5. [Contributing](#contributing)
6. [Roadmap](#roadmap)
7. [License](#license)

## Project Structure
- `data/`: Datasets and preprocessing scripts.
- `models/`: Pre-trained and fine-tuned models.
- `notebooks/`: Jupyter notebooks for experimentation.
- `src/`: Source code for TTS and STT systems.
- `tests/`: Unit and integration tests.
- `docs/`: Project documentation.

Here’s the repository is organize your to support iterative development for both TTS and STT

thoknaath/ <br>
├── .github/ # GitHub-specific files <br>
│ ├── workflows/ # CI/CD pipelines (e.g., testing, deployment) <br>
│ ├── ISSUE_TEMPLATE/ # Templates for GitHub issues  <br>
│ └── PULL_REQUEST_TEMPLATE.md # Template for PRs <br>
├── data/ # Datasets and preprocessing scripts <br>
│ ├── tts/ # TTS-specific data <br>
│ │ ├── raw/ # Raw text and audio files <br> 
│ │ ├── processed/ # Cleaned and preprocessed data <br>
│ │ ├── metadata.csv # LJSpeech-style metadata <br>
│ │ └── preprocess.py # Script for preprocessing TTS data <br>
│ └── stt/ # STT-specific data <br>
│ ├── raw/ # Raw audio and transcriptions <br>
│ ├── processed/ # Cleaned and preprocessed data <br>
│ ├── metadata.csv # CommonVoice-style metadata <br>
│ └── preprocess.py # Script for preprocessing STT data <br>
├── models/ # Pre-trained and fine-tuned models <br>
│ ├── tts/ # TTS models <br>
│ │ ├── pretrained/ # Pre-trained TTS models <br>
│ │ └── finetuned/ # Fine-tuned Nuer TTS models <br>
│ └── stt/ # STT models <br>
│ ├── pretrained/ # Pre-trained STT models <br>
│ └── finetuned/ # Fine-tuned Nuer STT models <br>
├── notebooks/ # Jupyter notebooks for experimentation <br>
│ ├── tts/ # TTS notebooks <br>
│ │ ├── data_exploration.ipynb # Explore TTS dataset <br>
│ │ └── model_training.ipynb # Train TTS models <br>
│ └── stt/ # STT notebooks <br>
│ ├── data_exploration.ipynb # Explore STT dataset <br>
│ └── model_training.ipynb # Train STT models <br>
├── src/ # Source code <br>
│ ├── tts/ # TTS-related scripts <br>
│ │ ├── preprocess.py # Data preprocessing for TTS <br>
│ │ ├── train.py # Model training for TTS <br>
│ │ ├── api.py # TTS API <br>
│ │ └── utils.py # Utility functions for TTS <br>
│ └── stt/ # STT-related scripts <br>
│ ├── preprocess.py # Data preprocessing for STT <br>
│ ├── train.py # Model training for STT <br>
│ ├── api.py # STT API <br>
│ └── utils.py # Utility functions for STT <br>
├── tests/ # Unit and integration tests <br>
│ ├── tts/ # TTS tests <br>
│ │ ├── test_preprocess.py # Test TTS preprocessing <br>
│ │ ├── test_train.py # Test TTS training <br>
│ │ └── test_api.py # Test TTS API <br>
│ └── stt/ # STT tests <br>
│ ├── test_preprocess.py # Test STT preprocessing <br>
│ ├── test_train.py # Test STT training <br>
│ └── test_api.py # Test STT API <br>
├── docs/ # Documentation <br>
│ ├── setup.md # Setup instructions <br>
│ ├── tts_guide.md # TTS development guide <br>
│ ├── stt_guide.md # STT development guide <br>
│ ├── contributing.md # Contribution guidelines <br>
│ └── roadmap.md # Project roadmap <br>
├── README.md # Project overview <br>
├── requirements.txt # Python dependencies <br>
└── LICENSE # Project license (e.g., MIT) <br>
  
## Getting Started
   ### Prerequisites
- Python 3.8 or higher
- Git
- A GPU (recommended for training models)

  ### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/thai22/thoknaath.git

2. Install dependencies:
   ```bash 
   pip install -r requirements.txt
### Set up the environment:
   - For TTS, follow the TTS Guide.
   - For STT, follow the STT Guide.

Follow the guides in docs/ to set up the TTS and STT systems.

## Usage
  ### TTS System
  - Preprocess the data:
     ```bash
        python src/tts/preprocess.py
  - Train the model:
     ```bash
        python src/tts/train.py
  - Run the TTS API:
     ```bash
        python src/tts/api.py
  - Send a POST request to /tts with Nuer text to synthesize speech.

  ### STT System
  - Preprocess the data:
    ```bash
    python src/stt/preprocess.py
  - python src/stt/train.py
    ```bash
    python src/stt/train.py
  - python src/stt/api.py
    ```bash
    python src/stt/api.py
  - Send a POST request to /stt with an audio file to transcribe speech.

## Development
### Data Collection
  - Add raw text and audio files to data/tts/raw/ and data/stt/raw/.
  - Use the preprocessing scripts (preprocess.py) to clean and prepare the data.
### Model Training
  - Use the training scripts (train.py) to fine-tune pre-trained models on the Nuer dataset.
  - Monitor training progress using TensorBoard or logs.


  ### Testing
  -  Run unit tests for TTS and STT:
        ```bash
            pytest tests/tts/
            pytest tests/stt/
## Contributing
We welcome contributions! Please read our Contribution Guidelines for details on how to:
  - Report issues.
  - Submit pull requests.
  - Add new features or improve documentation.
    
## Roadmap
Check out our Roadmap to see the planned features and milestones for ThokNaath.
## License
This project is licensed under the MIT License. See LICENSE for details.
## Acknowledgments
  - The Nuer-speaking community for their support and contributions.
  - Open-source tools like Coqui TTS, Hugging Face, and PyTorch for enabling this project.
## Contact
  - For questions or feedback, please open an issue or contact the project maintainers.
    
