# Voice_cloning_script
Estudely Voice cloning script submission
## YouTube Audio Downloader and Converter
This script allows you to download the audio from a YouTube video and convert it into a 16kHz mono WAV file. It handles invalid or incorrect URLs and provides an easy way to download the audio locally (especially useful for Google Colab and Jupyter Notebooks).

## Features
Downloads audio from any YouTube video via yt-dlp

Converts the audio to a 16kHz mono WAV file using ffmpeg

Handles invalid URLs and errors gracefully

Supports downloading the file locally or via Google Colab

## Requirements
Python 3.x

yt-dlp for downloading YouTube videos

ffmpeg for audio conversion

## Install Dependencies
You can install the required dependencies using pip:
pip install yt-dlp
On Linux or macOS, install ffmpeg using:


### sudo apt-get install ffmpeg
For Windows, download and install ffmpeg from the official website: FFmpeg Downloads

## How to Use
### 1. Clone this repository:

git clone https://github.com/
cd youtube-audio-downloader
2. Run the script:
python youtube_to_audio.py
3. Provide the YouTube video URL when prompted:
Enter YouTube video URL: https://www.youtube.com/watch?v=YOUR_VIDEO_ID
The script will:

Download the audio.

Convert it to a 16kHz mono WAV file.

Save it as output.wav in the current working directory.


### Error Handling
If an invalid YouTube URL is entered, an error message will be shown.

If there is an issue during the conversion, a descriptive error will appear.

Downloading the Audio Locally (Google Colab)
If you're using Google Colab, the audio file will automatically be available for download after processing. You can simply click on the download link when prompted.

If you're running the script on Jupyter Notebook or your local machine, the output.wav file will be saved in the same directory where the script is located.

