    # Unofficial ChatGPT API for python

    *WARNING - You will need to provide your OpenAI username and password for the bot to log in to the webpage.
    Do so at your own risk. Read the code and make sure it doesn't do anything fishy.
    
    This is NOT an official ChatGPT package. This is a hacky workaround for using chatGPT in python by opening up a headless browser. Don't rely on this for anything important.
    OpenAI changes their website frequently, so this will probably break often. The code should be simple enough for you to fix yourself though.
    *

    This class wraps a headless playwright browser instance that navigates to the chat.openai.com webpage and communicates with it for you.

    ---

    usage:

    ```
    chat = ChatGPT(openai_username, openai_password)

    # connect to the browser
    await chat.connect()

    # log in to the webpage
    await chat.login()

    response = await chat.send_message("Hello")
    print(response)
    ```