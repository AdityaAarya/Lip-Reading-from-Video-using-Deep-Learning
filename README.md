# LipRead - Deep Learning Lip Reading Application

LipRead is a sophisticated deep learning application that can read lips from mute videos using advanced computer vision and deep learning techniques. The project uses a combination of 3D CNNs and Bidirectional LSTMs to achieve accurate lip reading predictions.

## Features

- Real-time lip reading from video input
- Interactive web interface using Streamlit
- Support for video file upload and processing
- Visual feedback showing model's video processing
- Deep learning model with 3D CNNs and Bidirectional LSTMs

## Technology Stack

- **Python** - Primary programming language
- **TensorFlow** - Deep learning framework
- **Streamlit** - Web interface
- **FFmpeg** - Video processing
- **OpenCV** - Image processing

## Model Architecture

The deep learning model consists of:
- Multiple 3D Convolutional layers for spatial-temporal feature extraction
- MaxPooling layers for dimensionality reduction
- Bidirectional LSTM layers for sequence learning
- Dense layer with softmax activation for classification
- Dropout layers for regularization

## Project Structure

```
lip-reading/
├── app/
│   ├── modelutil.py      # Model architecture and loading
│   ├── streamlitapp.py   # Streamlit web application
│   ├── utils.py          # Utility functions
│   └── test_video.mp4    # Sample video for testing
├── models/
│   ├── checkpoint 50.zip # Model checkpoint at epoch 50
│   └── checkpoint 96.zip # Model checkpoint at epoch 96
└── LipRead.ipynb        # Jupyter notebook for model development
```

## Getting Started

### Prerequisites

- Python 3.9+
- TensorFlow
- Streamlit
- FFmpeg
- Required Python packages (see requirements below)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/AdityaAarya/Lip-Reading-from-Video-using-Deep-Learning.git
cd lip-reading
```

2. Install required packages:
```bash
pip install tensorflow streamlit imageio ffmpeg-python
```

3. Run the application:
```bash
cd app
streamlit run streamlitapp.py
```

## Usage

1. Launch the Streamlit application
2. Select a video file from the dropdown menu
3. The application will display:
   - Original video on the left
   - Processed frames used by the model on the right
   - Predicted text output below

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Thanks to the TensorFlow and Streamlit communities
- Special thanks to contributors and maintainers

---
**Note**: This project is for educational and research purposes. Results may vary depending on video quality and lighting conditions.
