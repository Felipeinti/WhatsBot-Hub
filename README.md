# WhatsBOT-HUB: AI-Powered WhatsApp Chat Responder

Welcome to WhatsBOT-HUB, a script that enables automated responses to WhatsApp messages using GPT-3 from OpenAI.

The script leverages several Python libraries to achieve its functionality. It listens for incoming WhatsApp messages, analyzes the text, and then generates an appropriate response using the GPT-3 model. The generated response is then sent back as a reply to the incoming message.

## How It Works

The script performs the following steps:

1. **WhatsApp Initialization**: Waits for 3 seconds, and then opens WhatsApp application.

2. **New Message Detection**: Periodically searches for new incoming messages in WhatsApp.

3. **Message Extraction**: If a new message is detected, it takes a screenshot of the message, and then processes the image to extract the text.

4. **Response Generation**: The extracted text is sent to GPT-3, which generates an appropriate response.

5. **Sending Reply**: The generated response is then sent back as a reply to the incoming message.

## Key Functions

Here are the core functions used in the script:

- **buscar_nuevo_mensaje()**: Searches for new incoming messages.

- **extraer_mensaje()**: Takes a screenshot of the new message and saves it.

- **leer_mensaje()**: Reads the text from the screenshot of the message.

- **buscar_respuesta()**: Sends the read text to the GPT-3 model and receives the generated response.

- **enviar_respuesta()**: Sends the generated response back as a reply to the incoming message.

## Prerequisites

Before running the script, you need to have the following installed:

- Python 3.x
- Tesseract-OCR
- OpenAI's GPT-3 API key

Python libraries: time, os, cv2, PIL, pyperclip, pyautogui, pyscreenshot, pytesseract, openai, configparser

## Installation

### Tesseract-OCR

Tesseract-OCR is used for Optical Character Recognition (OCR). You need to install it and specify the path in the script:

- For macOS: `/opt/homebrew/bin/tesseract`
- For Windows: `C:\Program Files\Tesseract-OCR\tesseract`

### OpenAI's GPT-3 API Key

You need to provide your API key for OpenAI's GPT-3. Place the key in a file named `login.ini`.

### Python Libraries

All required Python libraries can be installed via pip:

```shell
pip install opencv-python pillow pyperclip pyautogui pyscreenshot pytesseract openai configparser
```

## Running The Script

Run the script with Python:

```shell
python elprofealejo.py
```

Please note that the script is designed to work with a specific layout and might require adjustments based on your system resolution and WhatsApp layout. Ensure WhatsApp is running and is in the foreground for the script to work properly.

## Note

The script is designed for educational purposes and should not be used for spamming or other inappropriate behavior. Always respect the privacy and time of your contacts.
