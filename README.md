# Voice_cloning_script
Estudely Voice cloning script submission
## YouTube Audio Downloader and Converter
This script allows you to download the audio from a YouTube video and convert it into a 16kHz mono WAV file. It is designed to run on Google Colab, making it easy to use in a cloud environment without needing to install any dependencies locally. The script handles invalid or incorrect URLs and provides an easy way to download the audio locally.

## Features
Downloads audio from any YouTube video via yt-dlp

Converts the audio to a 16kHz mono WAV file using ffmpeg

Handles invalid URLs and errors gracefully

Designed to run on Google Colab, making it accessible in the cloud

Supports downloading the file locally to your system (via Colab)

## Requirements
Python 3.x

yt-dlp for downloading YouTube videos

ffmpeg for audio conversion

## Install Dependencies
You can install the required dependencies using pip:
pip install yt-dlp
On Linux or macOS, install ffmpeg

The required dependencies are automatically installed in Google Colab, but you can also install them manually if running locally.
## Install Dependencies (for Local Use)
If you're running this script locally (not on Colab), you can install the required dependencies using pip:

pip install yt-dlp
On Linux or macOS, install ffmpeg using:
sudo apt-get install ffmpeg
For Windows, download and install ffmpeg from the official website: FFmpeg Downloads

## How to Use
### For local script
### 1. Clone this repository:
git clone https://github.com/Bhalalaronak/Voice_cloning_script.git
cd Voice_cloning_script
### 2. Run the script:
python youtube_to_audio.py
### 3. Provide the YouTube video URL when prompted:
Enter YouTube video URL: https://www.youtube.com/watch?v=YOUR_VIDEO_ID
   . The script will:

   . Download the audio.

   . Convert it to a 16kHz mono WAV file.

  . Save it as output.wav in the current working directory.
## Using Google colab
### Open the youtube_to_audio.ipynb file in Google Colab:
Go to Google Colab.

### Open the youtube_to_audio.ipynb file from the cloned repository.

### Run the cells in the notebook:
First, execute the cell to install the required dependencies (yt-dlp and ffmpeg).

Next, run the cell where you input the YouTube video URL.

The script will download and convert the audio to a 16kHz mono WAV file.
### Provide the YouTube video URL when prompted:
Enter YouTube video URL: https://www.youtube.com/watch?v=YOUR_VIDEO_ID
The script will:

Download the audio.

Convert it to a 16kHz mono WAV file.

Save it as output.wav in the Colab environment.

## Error Handling
If an invalid YouTube URL is entered, an error message will be shown.

If there is an issue during the conversion, a descriptive error will appear.

## Downloading the Audio Locally (Google Colab)
If you're using Google Colab, the audio file will automatically be available for download after processing. You can download it using the files.download() method provided in Colab:
from google.colab import files
files.download("output.wav")
If you're running the script locally (in Jupyter Notebook or a local Python environment), the output.wav file will be saved in the same directory where the script is located.


