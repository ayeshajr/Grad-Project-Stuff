# Graduation Project Code - *Changelog* <!-- omit in toc -->

## Table of Contents <!-- omit in toc -->

- [Week 11](#week-11)
- [Week 10](#week-10)
- [Week 9](#week-9)
- [Week 8](#week-8)
- [Week 7](#week-7)
- [Week 5](#week-5)
- [Week 4](#week-4)
- [Week 3](#week-3)
- [Week 2](#week-2)

## Week 11

Mar 25:

- Restructured Saved Weights Folder
- Added 6 Models trained on data of 13 words and 4 people
  - 5 FPS x2 (Max Accuracy and Min Loss)
  - 9 FPS x2 (Max Accuracy and Min Loss)
  - 13 FPS x2 (Max Accuracy and Min Loss)
- Added Notebooks that were used for training and recording data

Mar 21:

- Added 4 Models trained on data of 13 words and 3 people
  - 25 FPS x2 (Max Accuracy and Min Loss)
  - 13 FPS
  - 9 FPS

- Added 2 Models trained on data of 13 words and 4 people
  - 25 FPS
  - 13 FPS

## Week 10

Mar 19:

- Alphabets added to NLP Dataset
- Added new NLP Model and Weights trained on new dataset

Mar 15:

- Added NLP weights to handle "Hello [Name]"

Mar 14:

- Added 2 Models trained on data of 10 words and 4 people
- Updated Script to Record CV Data - `CV_Model.ipynb`

## Week 9

Mar 6:

- Dataset changes
  - Combined 2 datasets (Dataset 1 and Dataset 2) into one dataset - `Dataset_1780_rows.csv`
  - Created a double version of the dataset
  - Fixed finger spelling placeholders
  - Added new sentences
- Updated NLP Script
  - Handles finger spelling now
  - Adds '?' after 6 W's and How
  - Fixed hardcoded values when initialing model
- Updated weights and `myVars.txt` for the NLP model

## Week 8

Mar 5:

- Updated NLP Script
  - Added function `preprocess_sentence` that will handle all preprocessing
  - Added code to handle finger spelling
  - Handling '?' (QM-wig) and manually adding ? to decoded sentence

Mar 3:

- Computer Vision Data Collection script updated
  - Added code to prompt action on screen while collecting data
- Uploaded the Updated version of `Main Notebook - Updated.ipynb`
- Uploaded new models in `Saved Weights` folder

Mar 1:

- Computer Vision data collection script changes
  - Removed useless Imports
  - Changed draw_landmarks (Face landmarks)
  - Added function (extract_keypoints)
  - Changed sequence length to 25 and number of sequences to 40

Feb 28:

- Added 2 new datasets for NLP

## Week 7

Feb 22:

- Uploaded 4 new models with training Camera position as Standing and Seated
- Updated `NLP_Model.py` so that it handles words that aren't part of the dictionary

Feb 21:

- Created new issues and assigned who needs to work on them
- Removed all additional Datasets

## Week 5

Feb 12:

- Added the `Computer Vision Model` folder
  - With `Notebooks` folder containing the main notebook and the saved weights
  - With `Scripts` folder containing 3 scripts for training data collection

- Restructured the `NLP Model` folder
  - Reduced the folder hierarchy for better easy navigation
  - Added a `ReadMe` file

Feb 11:

- Restructured the repository
- Added 2 Main folders for each Model; `NLP Model` and `Computer Vision Model`.

Feb 10:

- Added ReadMe file and small update to `NLP_Model.py`
  - ReadMe file for the `Scripts/Model` directory that shows how to use the NLP Model
  - `NLP_Model.py` now has a loop that keeps taking input

Feb 8:

- Major update to `NLP_Model.py`
  - Combined generate_batch function with decode_sequence and now it takes an user input instead of a dataset
  - Made it so that the python program can take an argument, this will be the ASL text
  - Removed unused imports
  - Added new colors for printing text
  - Removed code for importing and preprocessing dataset
  - Removing import to other file with functions, only 1 function was being used so it has now been moved to the file itself (read_list_from_file)
  - Added timing for all sections of the code
  - Removed all unnecessary code

Feb 6:

- Added a script for NLP model
  - Reorganized `Scripts` folder into 2 parts; Data & Model
    - `Scripts/Data` holds all the scripts related to data extraction
    - `Scripts/Model` holds the python code for the NLP model
  - Updated `Encoder_Decoder_V4` file to  save model in H4 format
  - Added `Scripts/Model` folder
    - `NLP_Model.py`: Refactored the python notebook code
    - `functions.py`: Unimportant functions moved to this
    - `myVars.txt`: Dependant variables that take the longest time to load are now saved in here (over a pkl file for readability)
    - Incomplete task: Change the decoder function code to take user inputs

## Week 4

Feb 5:

- Added Encoder_Decoder V4
  - Removed .pkl files as they are not required (check commit description for more details)
  - Added a file with the dataset rows doubled for testing

## Week 3

Jan 25:

- Dataset Addition from this site <https://www.lifeprint.com/asl101/index/sign-language-phrases.htm>
- Made changes to the Encoder_Decoder Notebook for the PoC Presentation

Jan 23:

- Dataset changes
  - Removing all maths sentences
  - Some sentences had 3 lines (removing those sentences)
- Fix for [removingSpacesFromDataset.py](removingSpacesFromDataset.py): Previous code wasn't iterating properly and was pasting the same sentences twice
- Reorganized repository

Jan 22: Added [Encoder_Decoder_V2.ipynb](Encoder_Decoder_V2.ipynb): 2nd Version of EncoderDecoder

Jan 20: New dataset added, has around 2K rows of data & script written by her

## Week 2

Jan 19: Updated python notebook with completed encoder-decoder code. Still needs a lot of improvements

Jan 17: Repo set up
