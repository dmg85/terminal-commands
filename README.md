# Terminal-commands 🧑🏻‍💻 x Linux/macOs

Repository with the list of the basic commands to operate from the terminal.

## Key Commands & Navigation

* `Up and Down` Will show your previously used commands
* `Tab key` Autocomplete your text
* `Ctrl+L` Clear your terminal screen
* `Ctrl+C` Cancel the command and go to the next line without executing anything
* `Ctrl+R` Will pop up a search box and is going to match the last command
* `Ctrl+D` Closes the terminal

## To learn about the commands :book:

* `man` Stands for manual command and shows the documentation of a certain command eg: man ls, to exit press q
* `whoami` Show the registered user
* `date` Show the current date

## Navigation :earth_americas:

* `pwd` Print the current working directory
* `ls` List out the content of a folder and you can add "-a" shows hidden files or "-l" will show extra information like permissions, and file size, but also allows you to combine them eg: `la -a -l`
* `cd` Changes your directory and also can be combined with the following commands:
  - `cd ..` Takes you one level up
  - `cd -`  Takes me back to the last folder I was in
  - `cd /`  Takes you to the root of your machine

## Open files & folders :open_file_folder:

* `open` Just type open and the name of the file including the extension or the folder
   - You can also open a URL's like this: open https://github.com + enter and that will open the website in your predefined browser

## Creating and modifying files and directories :bookmark_tabs:

* `mkdir` Creates a folder eg: __mkdir__ folder1
* `touch` Creates a file eg: __touch__ docs.txt
  - You can also create multiple files at the same time using the following syntax: (here we are creating 10 numbered files)
  
    ![Screen Shot 2023-05-20 at 7 56 34 PM](https://github.com/dmg85/terminal-commands/assets/69224630/bae7c955-fa59-4e02-a569-398abfbeb87f)

* `rm` Remove files eg: __rm__ folder1, and there's also other options:
  - `rm -i` Prompts you a message asking if you want to delete the file
  - `rm -r` To delete an empty folder
  - `rm -fr` To delete a folder with files in it

## Copying and moving files :truck:

* `cp` To copy a file into another folder eg: __cp__ docs.txt &nbsp;folder2/docs.txt
* `mv`To move to another folder eg: __mv__ index.html folder2/index.html
  - __mv__ also allows you to rename a folder or file eg: __mv__  source src
  - To move a file out of a folder and rename it: __mv__  insideFolder/ doc.txt info.txt
  
## Dealing with file content :abcd:

* `cat` a shorthand for concatenate, allows you to read the content of a file eg: cat foldername/file.js "Will show you the content of a file"
* `cat >` or just `> ` + name of the file to write to a file press enter and all the text you put in the next line(s) will be added to the file you've specified:
   - ![Screen Shot 2023-05-20 at 11 57 31 AM](https://github.com/dmg85/terminal-commands/assets/69224630/bc0abb31-1c83-45d7-a8e8-0f5a00809304)
   - To exit the editing of the file press `ctrl + d`
   - `>>` will append the file in a new line
   - `cat -n` will show line numbers
* `less` Shows the content of the file but also allows us to scroll up & down, `q` will exit the less mode.
*  `head` + filename  will show the first 10 lines by default 
  - `head -n` + [number] + filename, will show the number of lines you specify
  - `tail` will give you the last 10 lines by default and also `tail -n` + a number will give you that exact amount of lines
* `echo` will print out the text written after the command
  - You can also apply `echo` to a file using the following syntax:![Screen Shot 2023-05-20 at 7 32 45 PM](https://github.com/dmg85/terminal-commands/assets/69224630/09046bbc-9117-4095-b7a5-1f4467a779f3)


## Terminal-based editor (NANO) :arrows_clockwise:

* `nano` + filename, will open the editor allowing you to edit a file.
 - To escape nano press `ctrl + x` press __y__ or __n__ to save your changes
 - If you want to know more about the editor please visit [nano](www.nano-editor.org/docs.php)

## Searching tools :mag:

* `grep` command search for a specific line or pattern in a file, you should specify the line you are looking for inside double      quotes like this:

>![Screen Shot 2023-05-20 at 7 46 17 PM](https://github.com/dmg85/terminal-commands/assets/69224630/ee4a3a16-0e4c-4444-955b-8a5e915b0f51)

* `find` search for a file using regular expressions to define a search pattern, regular expressions a.k.a regex uses a combination of characters known as **Metacharacters** here are some of the most commonly used:
   - `.` (dot): Matches any single character except a newline
   - `*`: Matches zero or more occurrences of the preceding character or group
   - `+`: Matches one or more occurrences of the preceding character or group
 > ![Screen Shot 2023-05-20 at 8 11 59 PM](https://github.com/dmg85/terminal-commands/assets/69224630/f235bb21-5390-4781-a8c3-c84986f19ae0)

In the example above the "." represents the current directory and the "-name" indicates to find by name
- You can also search for empty files using the `-empty` command
- `find` . -name "file-*" -delete will delete all the files containing that name and the consecutive numbers eg: "file-001, file-002, file 003" etc

## Piping
   Is a form to redirect an output to another destination or a file, check the following example:
   - Let's say we are looking for files with the text "doc-0*" which were previously created using the touch and curly braces syntax `touch doc-{01..05}.txt` 
    
   > ![Screen Shot 2023-05-22 at 5 49 28 PM](https://github.com/dmg85/terminal-commands/assets/69224630/c3745bd8-61dc-405c-8d11-977651fc7ef8)
  
   -  In the image above we are indicating that the search result be outputted in the file after the ">", and this will be the result:
   
   >  ![Screen Shot 2023-05-22 at 6 00 33 PM](https://github.com/dmg85/terminal-commands/assets/69224630/f032012d-162d-4274-bda7-acc859b3c8bc)

## Create a symlink
   A symlink can be understood as a file that points to another file or folder, without the need to duplicate files in the case of folders.
   - In this case, we have a profiles folder located in the Documents folder containing some files inside
     
   > ![Screen Shot 2023-12-07 at 9 39 40 AM](https://github.com/dmg85/terminal-commands/assets/69224630/9bbf8340-8a13-4770-957f-e373787c4ffd)

   - Next, we type the link command "ln" + "-s" for symbolic then indicate where the folder is followed by the folder name, and finally the destination folder 

   > ![Screen Shot 2023-12-08 at 6 34 52 AM](https://github.com/dmg85/terminal-commands/assets/69224630/29028072-7d4f-434b-8290-b25bcc238a86)

   > ![Screen Shot 2023-12-08 at 6 45 39 AM](https://github.com/dmg85/terminal-commands/assets/69224630/1ab71c2b-22b3-4ca9-8168-11e95a51585d)
