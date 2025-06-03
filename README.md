Hey, fellow local LLMers.

I made this simple 20Kb HTML-based ollama client, since all the other clients available requires you to download Docker and what not. I didn't want that, nor did I want some sketchy third party app.

Despite being a single file HTML running in your browser, does offline most of what a normal online LLM chat client would be expected to do. You can also edit assistant responses in hindsight and laugh at the LLM being puzzled and apologizing profusely why it just cursed at you, and switch models mid conversation.

To me this has been quite useful, since it runs without anything else than a browser and ollama, so it fits well into the "offline movement". I hope you like it too.

All you have to do:

Download ollama.html from this link https://github.com/gustavtresselt/localllm/

Put it at your desktop or similarly, and dragdrop it into Chrome

Make sure Ollama is running in your system tray.

To allow Ollama to receive queries from this browser, you have to create an environment variable called OLLAMA_ORIGINS and set it to "*". It is quite simple on most systems. This is a potential security concern, but definitely not as bad as having Docker on your PC. Lets hope Ollama offers a better origin control later. But hey, who is connected to the internet anyway?

Use it, enjoy, modify as you see pleased ofc. About half the work of this was human, half was Gemini2.5. You can easily check it for vulnerabilities using a local or offline LLM, of course, and the code is human readable.

I will probably update it with support for image and animation generation later, but this probably requires a second service (python client) to manage huggingface image generation, so don't wait up.
