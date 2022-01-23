<div align="center">

# GPT-3 BOM IMPORTER

<img src='https://cdn-images-1.medium.com/max/1024/0*yr6iy3A_kA7SQ8PV.png' width=500px> <br>
source : https://towardsai.net/p/opinion/ai-copy-assistant-powered-by-gpt-3<br>

  
[About](#about) •
[Configuration Requirements](#configuration-requirements) •
[Installation](#installation) •
[What we did](#What we did)  
  
</div>

## 📒 About <a name="about"></a>

I created as part of a GPT-3 makethon held at my University - Technical University of Munich in the year 2021. When project was created GPT3 was still not available for the public, but as part of the makethon we were provided with the access.

This project was created using GPT-3, davinci QnA model. Wherein we trained GPT3 to extract electronics part-ID from the excel sheets. Usually every vendor uses own template within the excel sheet to list down the electronic-ID, it becomes really tedious if a company which provides logistic services is not able to extract the correct IDs from these excel sheets. Many a times the IDs are even missing. To solve this problem was a challenge, with the help of GPT3 we were successful in extracting the correct IDs from the excel sheets with 80 percent accuracy.

## 👨‍💻 Configuration Requirements <a name="configuration-requirements"></a>

What is the required configuration for running this code
1. OS - any
2. Python 3.7+
3. Python libraries - openai, json
4. Jupyter notebook

## 🖥️ Installation <a name="installation"></a>

The data and API keys are not provided as part of the privacy policy and hence this project cannot be installed.
Although you can have a look at the code to get some inspiration if youy are working on GPT3 models.

## ✍️ What we did <a name="What we did"></a>

- Step1: File converted from excel to CSV with the import command
- Step2: Getting the name of the csv file
- Step3 : Feeding the file to GPT3 for using as the document to extract information from
  - Convert to GPT3 accessible file format : {"text":"...","metadata":"..."}
  - Convert the output into jsonl
  - Create file and uploading for GPT3 to access later
- Step4: Get questions from the file and use find_index() to get the index of that question
- Step5: Find the index of the question from the txt file
- Step6: GPT3 in action to get the MPN
- Step7: Get the required MPN and index by running gpt3
- Step8: Get the MPN and index to be sent to validator
- Step9: Create a excel sheet with MPNs to be downloaded
