# Terminal-commands 🧑🏻‍💻 x macOs

Repository with the list of the basic commands to operate from the terminal.

## Key Commands & Navigation

* `Up and Down` Will show your previous used commands
* `Tab key` Autocomplete your text
* `Ctrl+L` Clear your terminal screen
* `Ctrl+C` Cancel the command and goes to the next line without executing anything
* `Ctrl+R` Will pop up a search box and is going to match the last command
* `Ctrl+D` Closes the terminal

## To learn about the commands :book:

* `man` Stands for manual command and shows the documentation of a certain command eg: man ls, to exit press q
* `whoami` Show the registered user
* `date`show the current date

## Navigation :earth_americas:

* `pwd` Print the curent working directory
* `ls` List out the content of a folder and you can add "-a" shows hidden files or "-l" will show extra information like premisions, file size, but also allows you tu combine them eg: `la -a -l`
* `cd` Changes your directory and also can be combined with the following commands:
  - `cd ..` Takes you one level up
  - `cd -`  Takes me back to the last folder I was in
  - `cd /`  Takes you to the root of your machine

## Open files & folders :open_file_folder:

* `open` Just type open and the name of the file including the extension or the folder
   - You can also open a URL's like this: open https://github.com + enter and that will open the website in your predefined browser

## Creating and modifying files and directories :bookmark_tabs:

* `mkdir` Creates a folder eg: __mkdir__ folder1
* `touch` Creates a file eg: __touch__ docs.txt or multiple files at the same time eg: __touch__ users.txt callbacks.js
* `rm` Remove files eg: __rm__ folder1, and there's also other options:
  - `rm -i` Prompts you a message asking if you want to delete the file
  - `rm -r` To delete an empty folder
  - `rm -fr`To delete a folder with files in it

## Copying and moving files :truck:

* `cp` To copy a file into another folder eg: __cp__ docs.txt &nbsp;folder2/docs.txt
* `mv`To move to another folder eg: __mv__ index.html folder2/index.html
  - __mv__ also allows you to rename a folder eg: __mv__  source src
  - To move a file out of a folder and rename it: __mv__  insideFolder/ doc.txt info.txt
  
## Dealing with file content :abcd:

* `cat` shorthand for concatenate, allows you to read the content of a file eg: cat foldername/file.js "Will show you the content of a file"
* `cat >` to write to a file. And right after the "> " add the name of your file press enter and all the text you put in the next line(s) will be added to the file you've specified:
   - ![Screen Shot 2023-05-20 at 11 57 31 AM](https://github.com/dmg85/terminal-commands/assets/69224630/bc0abb31-1c83-45d7-a8e8-0f5a00809304)
   - To exit the editing of the file press `ctrl + d`

