# chatgpt-command-suggestion
ChatGPT interface that suggests commandline commands

Usage: suggest <command description>

# Example:
´´´
suggest clone sda1 to /mnt/
Suggested command: dd if=/dev/sda1 of=/mnt/ image_name.img
Execute suggested command? (Y/n): n
No action taken.

suggest clone the files system from / to /mnt/
Suggested command: sudo rsync -aAXv / /mnt/ --exclude={/dev/*,/proc/*,/sys/*,/tmp/*,/run/*,/mnt/*,/media/*,/lost+found}
Execute suggested command? (Y/n): n
No action taken.
