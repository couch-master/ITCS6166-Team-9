# ITCS6166 Team-9
# MakeItTalk

## Team
Puneeth Manikanta Sai Panem​

Venkata Sai Rakesh Thatipakala ​

Aditya Sahithi Gunda​

Ashwitha Lingannagari​

## Project Overview
MakeItTalk is an innovative project that brings static images to life by animating them in sync with audio inputs. Using advanced machine learning techniques, this project allows for the creation of realistic talking animations from any static portrait, synchronized with any given audio.

## Key Features
- Dynamic Facial Animation: Animates static facial images to mimic speech, creating a lifelike talking effect.
- Audio Processing: Analyzes the audio input to extract speech features which guide the animation process.
- Customizable Settings: Offers parameters to adjust the animation intensity and mouth movements to better match the spoken audio.

## Project Deliverables
### Selected Paper
**Title:** MakeItTalk: Speaker-Aware Talking-Head Animation

**Repository:** [MakeItTalk](https://github.com/yzhou359/MakeItTalk)

Link to Google Colab with comments on every line of code - [Google Colab](https://colab.research.google.com/drive/1xsUl9pXBztPLdndlm34ed6r-yjN1SRvI?usp=share_link)

## Execution Instructions
Here are step-by-step guide to set up and run the "MakeItTalk" project:

1. **Clone the Repository:**
   ```
   !git clone https://github.com/yzhou359/MakeItTalk
   ```
  
2. **Install Dependencies:**
   ```
   !cd MakeItTalk
   !pip install -r requirements.txt
   ```
   
3. **Download Pre-trained Models:**
   Download the pre-trained models from google drive, and save them in directory (`examples/ckpt/`).
   ```
   !gdown -O MakeItTalk/examples/ckpt/ckpt_autovc.pth 1ZiwPp_h62LtjU0DwpelLUoodKPR85K7x
   !gdown -O MakeItTalk/examples/ckpt/ckpt_content_branch.pth 1r3bfEvTVl6pCNw5xwUhEglwDHjWtAqQp
   !gdown -O MakeItTalk/examples/ckpt/ckpt_speaker_branch.pth 1rV0jkyDqPW-aDJcj7xSO6Zt1zSXqn1mu
   !gdown -O MakeItTalk/examples/ckpt/ckpt_116_i2i_comb.pth 1i2LJXKp-yWKIEEgJ7C6cE3_2NirfY_0a
   !gdown -O MakeItTalk/examples/dump/emb.pickle 18-0CYl5E6ungS3H4rRSHjfYvvm-WwjTI
   ```
   
4. **Prepare Input Data:**
   
   Put test audio files under examples folder as well with .wav format.


6. **Test:**
   ```
   python main_end2end.py --jpg <portrait_file>
   ```
   Make sure to provide a image file (portrait_file) containing the target person's face where lip-syncing will be applied.

7. **Check Outputs:**
   
   Ouput video is saved as out.mp4

### Demo
For a quick demo of what MakeItTalk can do, check out the following animation: [Video Demo](https://drive.google.com/file/d/1eDbBIVTLXY-NStbOjBOazZIBVKIV4M7X/view?usp=sharing)

### Project Presentation
[Project Presentation](https://docs.google.com/presentation/d/1pufIkySKLu1pQss6zeeFqnQeNVlBNPDx/edit#slide=id.g2d9bf514666_1_8)
