# Chatbot-With-Pytorch

# Implementation of a Contextual Chatbot in PyTorch.  
Simple chatbot implementation with PyTorch. 

- The implementation is with a Feed Forward Neural net with 2 hidden layers.

## Installation

### Create an environment
Whatever you prefer (e.g. `conda` or `venv`)
```console
mkdir myproject
$ cd myproject
$ python3 -m venv venv
```

### Activate it

Windows:
```console
venv\Scripts\activate
```
### Install PyTorch and dependencies

You also need `nltk`:
 ```console
pip install nltk
 ```
If you get an error during the first run, install `nltk.tokenize.punkt`:
Run this once in your terminal:
 ```console
$ python
>>> import nltk
>>> nltk.download('punkt')
```

### Usage
Run
```console
python train.py
```
This will dump `data.pth` file. And then run
```console
python chat.py
```

### intents.json
```console
{
  "intents": [
    {
      "tag": "greeting",
      "patterns": [
        "Hi",
        "Hey",
        "How are you",
        "Is anyone there?",
        "Hello",
        "Good day"
      ],
      "responses": [
        "Hey :-)",
        "Hello, thanks for visiting",
        "Hi there, what can I do for you?",
        "Hi there, how can I help?"
      ]
    },
    ...
  ]
}
```
