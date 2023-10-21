# Voice Guided Sample Aliquoting on Google Colab

## Overview
This tool offers a voice-assisted method for sample aliquoting. It guides the user through the process of aliquoting using voice commands, effectively reducing the chances of errors during the process. Built to run exclusively on Google Colab, it uses the platform's microphone access to capture user input and generate corresponding voice responses.

## Pre-requisites
* Google Colab environment
* Microphone access (a prompt will request for this when running the code)

## Setting Up
* Prepare Your Data: Modify the content of Template.csv to match your sample data. Retain the filename as "Template.csv". The format of your CSV should resemble:
```python
Metabolite1,Metabolite2
Value1,Value2
Value3,Value4
```

Example:
```python
Water,PEG
3.2,3.2
6.4,6.4
...
0.8,4.8
```

* Upload the File: Upload the modified Template.csv to your Google Colab environment.
* Run the Code: Execute the given code cell-by-cell in Google Colab.

## How to Use
1. After setting up, the code will install necessary packages.
2. Once everything is ready, you'll hear a voice command that indicates the beginning of aliquoting for a given metabolite.
3. The Colab interface will display the volume to aliquot and the sample number. You'll be directed on which sample to aliquot using voice commands.
4. Say "next" after you're done aliquoting a sample to proceed to the next one. Say "skip" if you wish to move onto the next metabolite without finishing the current one.
5. The process will continue until all samples for all metabolites are aliquoted or until you decide to skip.

## Important Notes
* Ensure your microphone is working properly and that the environment isn't too noisy for clear voice commands.
* The tool uses Google's speech recognition; hence, an active internet connection is required.
* Each recording segment waits for 5 seconds to capture your voice command. Adjust the step_sec parameter if you need more or less time.

> Remember, this tool is aimed to assist and guide you in the aliquoting process. Always double-check your work for best results!