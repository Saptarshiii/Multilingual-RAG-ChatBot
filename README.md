# Multilingual-RAG-ChatBot
## Overview
This is a Multilingual ChatBot that will provide response only for a given specific context. The context can be customized and read through a pdf file. The user can provide prompt in any language out of 99+ languages supported by Whisper AI.

## Features
Takes *live/pre-recorded* audio input
Provides AI-Generated Response only on the context provided

## Installation
### Clone this repository:
```
https://github.com/Saptarshiii/Multilingual-RAG-ChatBot.git

```
### Install the required dependencies:
```
pip install -r requirements.txt

```
## Usage
Linearly execute all the cells
After successful execution of all cells the last cell will launch the UI and there we can use the model

The Default context is about Rabindranath Tagore loaded in dummy.pdf
Write your custom context(knowledge about the topic the AI should answer) in any pdf and change the following variable
## Note: Make sure the dummy.pdf is present in the same folder as the notebook or you can use your own pdf as follows
```
pdf_path = "dummy.pdf"
#replace dummy.pdf with the name of your context file

```
You can alter the Temperature of the Gemini-Pro Model.
Temperature basically controls the randomness of the response i.e. it controls the creativity
```
cmodel = ChatGoogleGenerativeAI(model="gemini-pro", temperature=0.3, google_api_key=api_key)
#the range of temperature is 0.0-2.0

```
## License 
This project is licensed under the MIT License.
