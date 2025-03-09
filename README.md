# ThokNaath
open-source TTS and STT systems for the Nuer language to empower communication, education, and cultural preservation.


Here’s the repository is organize your to support iterative development for both TTS and STT
thoknaath/
├── .github/                  # GitHub-specific files (e.g., workflows, issue templates)
├── data/                     # Datasets and preprocessing scripts
│   ├── tts/                  # TTS-specific data (text-audio pairs)
│   │   ├── raw/              # Raw text and audio files
│   │   ├── processed/        # Cleaned and preprocessed data
│   │   └── metadata.csv      # LJSpeech-style metadata
│   └── stt/                  # STT-specific data (audio-text pairs)
│       ├── raw/              # Raw audio and transcriptions
│       ├── processed/        # Cleaned and preprocessed data
│       └── metadata.csv      # CommonVoice-style metadata
├── models/                   # Pre-trained and fine-tuned models
│   ├── tts/                  # TTS models
│   └── stt/                  # STT models
├── notebooks/                # Jupyter notebooks for experimentation
│   ├── tts_experiments.ipynb # TTS prototyping
│   └── stt_experiments.ipynb # STT prototyping
├── src/                      # Source code
│   ├── tts/                  # TTS-related scripts
│   │   ├── preprocess.py     # Data preprocessing for TTS
│   │   ├── train.py          # Model training for TTS
│   │   └── api.py            # TTS API
│   └── stt/                  # STT-related scripts
│       ├── preprocess.py     # Data preprocessing for STT
│       ├── train.py          # Model training for STT
│       └── api.py            # STT API
├── tests/                    # Unit and integration tests
│   ├── tts/                  # TTS tests
│   └── stt/                  # STT tests
├── docs/                     # Documentation
│   ├── setup.md              # Setup instructions
│   ├── tts_guide.md          # TTS development guide
│   └── stt_guide.md          # STT development guide
├── README.md                 # Project overview
└── requirements.txt          # Python dependencies
