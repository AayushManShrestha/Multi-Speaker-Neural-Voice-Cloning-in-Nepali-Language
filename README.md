# Multi-speaker Nepali Voice Cloning in Nepali Langauge
## Demo Video Link: [Minor Project Demo Video](https://www.youtube.com/watch?v=UYX3VjIn17U)

## Tacotron2 Fine-tuning Instructions

1. ```python
   !git clone https://github.com/AayushManShrestha/Multi-Speaker-Neural-Voice-Cloning-in-Nepali-Language.git
3. ```python
   import os
   os.chdir('Multi-Speaker-Neural-Voice-Cloning-in-Nepali-Language')
   !git submodule init
   !git submodule update
   !pip install -q unidecode tensorboardX

4. Upload wav file on drive then
   ```python
   !cp -r /content/drive/MyDrive/wav.zip /content/Multi-Speaker-Neural-Voice-Cloning-in-Nepali-Language
6. ```python
   !unzip wav.zip

8.  To train type this code **CAREFUL ON THE FILEPATH HERE**
   ```python
!python train.py --output_directory=<drivelink> --log_directory=<drivelink> -c <last_checkpointfile> --warm_start
