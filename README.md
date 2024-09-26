# Chatbot Api with fastapi

## Initial Setup:
This repo currently contains the starter files.

Clone repo and create a virtual environment
```
$ git clone https://github.com/thekbbohara/chatbotv1.git
$ cd chatbotv1
$ python3 -m venv venv
```
activate venv
```
$ . venv/script/activate #windows
$ source venv/bin/activate #linux

```

Install dependencies
```
$ (venv) pip install -r req.txt
```
Install nltk package
```
$ (venv) python
>>> import nltk
>>> nltk.download('punkt')
>>> nltk.download('punkt_tab')
```
Modify `intents.json` with different intents and responses for your Chatbot

Run
```
$ (venv) python train.py
```
This will dump data.pth file. And then run
the following command to test it in the console.
```
$ (venv) uvicorn app:app --reload

```

