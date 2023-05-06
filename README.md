# All In One Chatbot

This is a  chatbot created using the OpenAI API to generate responses to user inputs. It uses the `text-davinci-003` model to generate responses.

## Installation

1. Clone the repository
2. Install dependencies
`pip install -r requirements.txt`


## Usage

1. Run the script
`python main.py`

2. Go to your browser and open the link displayed on the terminal.
![Screenshot 2023-05-06 120146](https://user-images.githubusercontent.com/55046031/236606967-f9b51ece-aa1b-43a0-8699-ff99fb1c9337.png)

Get Two link One is works on LOcally and Other link Works On Cloud Shareable link

3. Type in your message and hit "SEND".

4. The chatbot will generate a response based on your message.

5. Continue the conversation by entering more messages.

6. To stop the script, press `Ctrl+C`.

## Gradio Interface

The Gradio interface consists of a textbox where you can input your messages and a chatbot window that displays the chat history. The chat history shows the conversation between you and the chatbot.

## Hosting

You can host the chatbot on your own server or cloud instance by running the script and exposing the port to the internet.

Alternatively, you can use the `share()` function provided by Gradio to host the chatbot on their servers. The `share()` function generates a link that you can share with others to use the chatbot.

```python
import gradio as gr

# define the chatbot
...
# create the Gradio interface
...
# launch the interface using Gradio's share() function
link = gradio.Interface.fn_name.share()
print("Shareable link:", link) 

```

## API Key
To use OpenAI's GPT-3 API, you must have a valid API key. The API key is stored as an environment variable. Alternatively, you can directly assign the key to openai.api_key as shown in the main.py file.

If you do not have an API key, you can sign up for a free trial [here](https://beta.openai.com/signup/).
