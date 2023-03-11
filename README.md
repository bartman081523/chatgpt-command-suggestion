# chatgpt-command-suggestion
ChatGPT interface that suggests Linux commandline commands based on a natural-language description

# Installation
git clone https://github.com/bartman081523/chatgpt-command-suggestion

-paste your OpenAI API key in the "suggest" file as 

openai.api_key = "YOUR_API_KEY"

sudo apt install python3-pip

sudo pip install openai

cd chatgpt-command-suggestion

sudo cp suggest /usr/bin/suggest


Usage: suggest (command description)

# Example:

suggest clone the files system from / to /mnt/

Suggested command: sudo rsync -aAXv / /mnt/ --exclude={/dev/*,/proc/*,/sys/*,/tmp/*,/run/*,/mnt/*,/media/*,/lost+found}

Execute suggested command? (Y/n): n

No action taken.


suggest grep the log for kernel errors

Suggested command: dmesg | grep "error"

Execute suggested command? (Y/n): n
