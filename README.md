# chatgpt-command-suggestion
ChatGPT interface that suggests commandline commands

# Installation
git clone https://github.com/bartman081523/chatgpt-command-suggestion
sudo pip install openai
cd chatgpt-command-suggestion
sudo cp suggest /usr/bin/suggest


Usage: suggest <command description>

# Example:

suggest clone sda1 to /mnt/

Suggested command: dd if=/dev/sda1 of=/mnt/ image_name.img

Execute suggested command? (Y/n): n

No action taken.


suggest clone the files system from / to /mnt/

Suggested command: sudo rsync -aAXv / /mnt/ --exclude={/dev/*,/proc/*,/sys/*,/tmp/*,/run/*,/mnt/*,/media/*,/lost+found}

Execute suggested command? (Y/n): n

No action taken.
