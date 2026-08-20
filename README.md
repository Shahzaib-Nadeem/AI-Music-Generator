# 🎵 AI Music Generator

An AI-based music generation system built with **Python, TensorFlow, Keras, and music21**. The project uses an **LSTM neural network** to learn patterns from MIDI music data and generate new musical sequences.

## 🚀 Features

* MIDI file processing
* Musical note and chord extraction
* Sequence preparation for machine learning
* LSTM-based music generation
* Neural network training
* Randomized music generation using temperature sampling
* Automatic MIDI file creation

## 🛠️ Technologies

* Python
* TensorFlow
* Keras
* NumPy
* music21
* MIDI
* LSTM Neural Networks

## 📁 Project Structure

```text
AI-Music-Generator/
│
├── music_generator.py
├── requirements.txt
├── README.md
├── .gitignore
│
└── midi_songs/
    └── *.mid
```

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/AI-Music-Generator.git
cd AI-Music-Generator
```

Install the required libraries:

```bash
pip install -r requirements.txt
```

## 🎼 Add MIDI Files

Create a folder named:

```text
midi_songs
```

Place your `.mid` files inside this folder.

Example:

```text
midi_songs/
├── song1.mid
├── song2.mid
└── song3.mid
```

The program reads these MIDI files and extracts notes and chords for training.

## ▶️ Run the Project

Run:

```bash
python music_generator.py
```

The program will:

1. Load MIDI files.
2. Extract musical notes and chords.
3. Prepare sequences for training.
4. Build the LSTM neural network.
5. Train the model.
6. Generate a new musical sequence.
7. Save the generated music as `output.mid`.

## 🧠 How It Works

The project follows this pipeline:

```text
MIDI Files
    ↓
Note & Chord Extraction
    ↓
Sequence Preparation
    ↓
LSTM Neural Network
    ↓
Model Training
    ↓
Music Generation
    ↓
MIDI Output
```

The model receives a sequence of musical notes and learns to predict the next note. After training, the model repeatedly predicts new notes to create a musical sequence.

## 📊 Model Architecture

The neural network consists of:

* LSTM layer — 256 units
* Dropout — 30%
* LSTM layer — 256 units
* Dropout — 30%
* Dense layer — 256 units
* Dropout — 30%
* Output layer with Softmax activation

The model uses the **Adam optimizer** and **categorical cross-entropy loss**.

## 🎶 Output

After successful execution, the generated music is saved as:

```text
output.mid
```

The MIDI file can be opened using software that supports MIDI playback.

## 👨‍💻 Author

**Shahzaib Nadeem**

BS Computer Science
Sir Syed University of Engineering and Technology, Karachi

## 📌 Future Improvements

* Add a graphical user interface.
* Improve music quality using larger datasets.
* Add multiple music genres.
* Save and load trained models.
* Add adjustable generation length and temperature.
* Generate different instruments and musical styles.
